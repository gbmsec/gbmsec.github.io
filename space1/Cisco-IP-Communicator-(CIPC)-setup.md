Example scenario: someone works from home on laptop and needs to make calls from office phone.


## Step-by-step guide

1. Download installer from [https://bit.ly/bcs-cisophone](https://bit.ly/bcs-cisophone) directly to user's workstation and install 

 **Troubleshooting** : Local antivirus might be blocking outgoing packets, e.g. Kaspersky Host Intrusion requires CIPC to be in Trusted group in order to work properly

 **Also** : If default installation did not work, set up in Windows XP SP3 compatibility mode




1. Run Cisco AnyConnect VPN client
    1. ld4-enter.bcsgm.com
    1. group: vpn-user

    
1. Run CIPC as administrator

    

    
1. Go to Preferences > Network
    1. Set TFTP address to 10.10.132.254
    1. Set 'Use this device name' (without spaces/dots) to SEPxxxxxxxxxxxx where x stands for [Softphone MAC address](http://click/it/_layouts/15/xlviewer.aspx?id=/it/Doc+Library/Softphones.xlsx) (link to Click/it/Softphone.xlsx

    

    

If MAC address is not present in the spreadsheet, request one from Network Team 



    









*****

[[category.storage-team]] 
[[category.confluence]] 
