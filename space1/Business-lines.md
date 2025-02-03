

SparklineBucketdd M yy1605783757490_-1452057158365|5|8|y w d h m|y w d h mANDPoint (.)0

INLINEimport groovy.json.JsonSlurper
import org.apache.commons.codec.binary.Base64
import org.apache.log4j.Level
import org.apache.log4j.Logger
 
def getUserInfo(String identifier){
    def post = new URL("http://jira/rest/api/2/user?key=${identifier}").openConnection();
    def authString = "jira_inc_mgmt_user:Z;e+7H9_5H";
    byte\[] authEncBytes = Base64.encodeBase64(authString.getBytes())
    String authStringEnc = new String(authEncBytes)
    def AUTH_HASH = "Basic ${authStringEnc}";
 
    post.setRequestMethod("GET")
    post.setDoOutput(true)
    post.setRequestProperty("Content-Type", "application/json")
    post.setRequestProperty("Authorization", AUTH_HASH)
    def postRC = post.getResponseCode();
    
 
    if (postRC.equals(200)) {
        def jsonSlurper = new JsonSlurper()
        def json = jsonSlurper.parseText(post.getInputStream().getText())
        def userInfo= json;
        return json.displayName
    } else {
        post = new URL("http://jira/rest/api/2/user?username=${identifier}").openConnection();
        post.setRequestMethod("GET")
        post.setDoOutput(true)
        post.setRequestProperty("Content-Type", "application/json")
        post.setRequestProperty("Authorization", AUTH_HASH)
        postRC = post.getResponseCode();

 
        if (postRC.equals(200)) {
            def jsonSlurper = new JsonSlurper()
            def json = jsonSlurper.parseText(post.getInputStream().getText())
            def userInfo= json;
            return json.displayName
        } else {
            return identifier
        }
    }
}

def printAssets(queryToPostJson) {
 
    def post = new URL("http://jira/rest/jip-api/1.0/index/query").openConnection();
    def authString = "jira_inc_mgmt_user:Z;e+7H9_5H";
    byte\[] authEncBytes = Base64.encodeBase64(authString.getBytes())
    String authStringEnc = new String(authEncBytes)
    def AUTH_HASH = "Basic ${authStringEnc}";
 
    post.setRequestMethod("POST")
    post.setDoOutput(true)
    post.setRequestProperty("Content-Type", "application/json")
    post.setRequestProperty("Authorization", AUTH_HASH)
    post.getOutputStream().write(queryToPostJson.getBytes("UTF-8"));
    def postRC = post.getResponseCode();
    def result = '';
 
    if (postRC.equals(200)) {
 
        def jsonSlurper = new JsonSlurper()
        def json = jsonSlurper.parseText(post.getInputStream().getText())
        def assets = json.assets;
 
        def headerRow = '';
        //headerRow += '<td>Asset ID</td>';
        headerRow += '<td>Name</td>';
        //headerRow += '<td>Type</td>';
        //headerRow += '<td>Create Date</td>';
 
        def isHeaderRowSet = false;
        //println(assets)
        if (assets != null) {
            assets.each { asset ->
              def disabled = false
              asset.inventoryItems.each { assetItem ->
                   //println(assetItem)
                   if (assetItem.attributeName in \["Disabled","Disaled"]){                     
                     if (assetItem.textValues?.contains("Yes")){
                        disabled = true
                     }
                   }
              }
              if (!disabled){
                def oneRow = '';
                //oneRow += '<td><a href="' + "http://jira/secure/DashboardAIPAction!default.jspa#/browse/"  + asset.id + '">' + asset.id + '</a></td>';
                oneRow += '<td>' + asset.name + '</td>';
                //oneRow += '<td>' + asset.formName + '</td>';
                //oneRow += '<td>' + asset.createdFormatted + '</td>';
                asset.inventoryItems.each { assetItem ->
                    //oneRow += assetItem //
                    //println(assetItem.attributeName)
                    if (assetItem.attributeName in \["BL Head", "Deputy", "Bucket", "Environment"]){
                      if (assetItem.attributeName in \["BL Head", "Deputy"]) {
                         if (assetItem.textValues){
                            
                             oneRow += '<td>' + getUserInfo(assetItem.textValues) + '</td>';
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
                        headerRow += '<td>' + assetItem.attributeName + '</td>';
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
 

println('<h3>Business lines</h3>');
def queryToPostJson2 = '{"searchType": "basic","listType": "detail","genericKeyword": null, "queryIndexSearchParams": \[{"field":"form.id","keywords":\[14],"fieldType":"LIST"}],"pageNumber": 1,"pageSize": 100,"sortDirection": "asc","sortField": "asset.name","sortType": "STRING","respTime": 1558685025363}';
printAssets(queryToPostJson2);





*****

[[category.storage-team]] 
[[category.confluence]] 
