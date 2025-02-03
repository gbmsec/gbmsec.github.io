"

,,,,,,,,false‚SparklineFiltration panelfalse,,true150,250,150falsefalsefalsetrue1699424857799_-17391914080,2,1falsefalse,false,falseService,EnvironmentfalsePoint (.)Service‚Environment‚Filter whole tableOR,ORdd M yyfalse365|5|8|y w d h m|y w d h mAND

INLINEimport groovy.json.JsonSlurper
import org.apache.commons.codec.binary.Base64
import org.apache.log4j.Level
import org.apache.log4j.Logger


def getWorkgroups(){
    def post = new URL("http://jira/rest/jip-api/1.0/index/query").openConnection();
    String authStringEnc = "amlyYV9pbmNfbWdtdF91c2VyOlo7ZSs3SDlfNUg="
    def AUTH_HASH = "Basic ${authStringEnc}";

    def queryToPostJson = '{"searchType": "basic","listType": "detail","genericKeyword": null, "queryIndexSearchParams": \[{"field":"form.name","keywords":\["Workgroup"],"fieldType":"LIST"}],"pageNumber": 1,"pageSize": 100,"sortDirection": "asc","sortField": "asset.name","sortType": "STRING","respTime": 1558685025363}';
 
    post.setRequestMethod("POST")
    post.setDoOutput(true)
    post.setRequestProperty("Content-Type", "application/json")
    post.setRequestProperty("Authorization", AUTH_HASH)
    post.getOutputStream().write(queryToPostJson.getBytes("UTF-8"));
    def postRC = post.getResponseCode();
    def result = \[:];
    if (postRC.equals(200)) {
         def jsonSlurper = new JsonSlurper()
         def json = jsonSlurper.parseText(post.getInputStream().getText())
         def assets = json.assets;
         assets.each { asset ->
                 asset.inventoryItems.each { assetItem ->
                    //oneRow += assetItem //
                    if (assetItem.attributeName == "Email"){
                        def email = assetItem.textValues;
                        if (email){
                            result.put(asset.name, '<a href="mailto:' + assetItem.textValues + '">'  + assetItem.textValues + '</a>');
                        } else {
                            result.put(asset.name, "");
                        }
                        
                    }
                 }
             
         }
    }
    //println(result );
     return result;
}
 
def printAssets(queryToPostJson) {
 
    def post = new URL("http://jira/rest/jip-api/1.0/index/query").openConnection();
    String authStringEnc = "amlyYV9pbmNfbWdtdF91c2VyOlo7ZSs3SDlfNUg="
    def AUTH_HASH = "Basic ${authStringEnc}";
    def liveStatuses = \["Live", "In Progress", "Target", "In Transition", "Non-target", "Approval required","External"]
 
    post.setRequestMethod("POST")
    post.setDoOutput(true)
    post.setRequestProperty("Content-Type", "application/json")
    post.setRequestProperty("Authorization", AUTH_HASH)
    post.getOutputStream().write(queryToPostJson.getBytes("UTF-8"));
    def postRC = post.getResponseCode();
    def result = '';
    if (postRC.equals(200)) {
        def workgroups = getWorkgroups();
 
        def jsonSlurper = new JsonSlurper()
        def json = jsonSlurper.parseText(post.getInputStream().getText())
        def assets = json.assets;
        //println(assets)
        //return
        def headerRow = '';
        headerRow += '<td>Service</td>';
        //headerRow += '<td>Name</td>';
        //headerRow += '<td>Type</td>';
        //headerRow += '<td>Create Date</td>';
 
        def isHeaderRowSet = false;
        if (assets != null) {
   
   
            assets.each { asset ->
                def live = asset.inventoryItems.find { assetItem ->
                    if (assetItem.attributeName == "State V2"){
                        assetItem.textValues in liveStatuses
                    }
                }
                if (live) {
                def oneRow = '';
																																																		  
                oneRow += '<td><a href="' + "http://jira/secure/DashboardAIPAction!default.jspa#/browse/"  + asset.id + '">' + asset.name + '</a></td>';

                //oneRow += '<td>' + asset.name + '</td>';
                //oneRow += '<td>' + asset.formName + '</td>';
                //oneRow += '<td>' + asset.createdFormatted + '</td>';
                asset.inventoryItems.each { assetItem ->
                    //oneRow += assetItem //
                    if (assetItem.attributeName in \["Business owner", "IT Owner", "CriticalityClass","Service Type","DetailedArch", "ServiceWorkingHours", "ServiceSupportWorkingHours", "IT Service Support Group", "Environment"]){
                      if (assetItem.attributeName in \["IT Service Support Group","DetailedArch"]) {
                         if (assetItem.textValues){

							 if (assetItem.attributeName == "Jira project key"){
                                 oneRow += '<td><a href="http://jira/projects/' + assetItem.textValues + '">'  + assetItem.textValues + '</a></td>';
                             } else 
                             	   if (assetItem.attributeName == "IT Service Support Group"){
                                          oneRow += '<td>' +  workgroups.get(assetItem.textValues) + '</td>';
                                      
                                 //oneRow += '<td><a href="mailto:' + assetItem.textValues + '">'  + assetItem.textValues + '</a></td>';
									} else{
                                 oneRow += '<td><a href="' + assetItem.textValues + '">link</a></td>';
                             }
                         } else {
                             oneRow += '<td> </td>';
                         }                       
                      } else {
                        if (assetItem.textValues){
                          oneRow += '<td>' + assetItem.textValues + '</td>';
                        } else {
                          oneRow += '<td> </td>';
                        }
                      }
                      if (!isHeaderRowSet) {
                        def headerName = assetItem.attributeName
                        if (assetItem.attributeName == "CriticalityClass"){
                           headerName  = "Criticality"
                        } else if (assetItem.attributeName == "ServiceSupportWorkingHours"){
                           headerName  = "Support working hours"
                        } else if (assetItem.attributeName == "ServiceWorkingHours"){
                           headerName  = "Service working hours"
                        } else if (assetItem.attributeName == "IT Service Support Group"){
                           headerName  = "Email"
                        }
                        headerRow += '<td>' + headerName  + '</td>';
                      }
                    }
                }
                if (!isHeaderRowSet) {
                    isHeaderRowSet = true;
                    result += '<thead><tr style="background-color: #e1e4e8; font-weight:bold">' + headerRow + '</tr></thead>\n';
                }
                result += '<tr>' + oneRow + '</tr>\n';
            }
            }
        }
//println(headerRow);
    }
    
    println('<table>' + result + '</table>');
}
 
println('<style> '+
        ' table { '+
        '   border-collapse: collapse; '+
        ' } '+
        ' th, td { '+
        '   border: 1px solid #ededed; '+
        '   padding: 10px; '+
        '   text-align: left; '+
        ' } '+
        ' </style>');
 

println('<h3>IT Services</h3>');
def queryToPostJson2 = '{"searchType": "basic","listType": "detail","genericKeyword": null, "queryIndexSearchParams": \[{"field":"form.name","keywords":\["Services V2"],"fieldType":"LIST"}],"pageNumber": 1,"pageSize": 400,"sortDirection": "asc","sortField": "asset.name","sortType": "STRING","respTime": 1558685025363}';
printAssets(queryToPostJson2);












*****

[[category.storage-team]] 
[[category.confluence]] 
