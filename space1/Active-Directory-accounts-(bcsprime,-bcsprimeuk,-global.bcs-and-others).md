

From technical point of view we have two sets of Active Directory (AD) domains:


* GMIB (Global Markets Investment Bank): bcsprime, bcsprimeuk. bcsprimecy, bcsprimeusa and possibly others.
* BCS Group: global.bcs (primary one), org-bcs and possibly others. 




## GMIB domains: bcsprime, bcsprimeuk. bcsprimecy, bcsprimeusa.
Primary domains for colleagues in GMIB. Each colleague has a primary account in one (and only one) of the domains. Only this primary AD account should be provided with permissions.

Managed by the GMIB Server admins team. Contact: [sd.srv@bcsgm.com](mailto:sd.srv@bcsgm.com) 

For some technical reasons (more on this below) users might have more than one account or accounts in several domains.


* bcsprime:
    * primary account for all Russia-based users.
    * Linked mailbox accounts for UK and US-based users in OU=bcsprime.local/bcsprime/UK/Users Mailboxes and OU=bcsprime.local/bcsprime/USA/Users Mailboxes. These are disabled by default and used only for emails. These accounts need to be added to distribution groups.  **Other permissions (security groups membership) must not be granted!** 
    * Rocket chat (only for rc.bcsgm.com) accounts for UK users in OU=bcsprime.local/bcsprime/UK/Users

    
* bcsprimeuk - primary account for all UK-based users.
* bcsprimecy - primary account for all Cyprus-based users.
* bcsprimeusa - primary account for all US-based users.




## Group: global.bcs
This account us ised for Group resources (cost.global.bcs, doc.global.bcs, Rocket chat rc.bcs.ru and others).

Managed by the Group IT (Отдел сопровождения windows сервисов). Contact: [sd@bcs.ru](mailto:sd@bcs.ru) 

Set to expire every 3 months. Password can be reset or updated on [https://pw.global.bcs/RDWeb/Pages/ru-ru/password.aspx](https://pw.global.bcs/RDWeb/Pages/ru-ru/password.aspx) 




### Account operator Rights.
Account operator rights (password resets) were granted to some colleagues in GMIV Service Desk. Contact [servicedesk@bcsgm.com](mailto:servicedesk@bcsgm.com) if you need to reset your global.bcs password


### Mapping between global.bcs and GMIB accounts.
[https://ekd.global.bcs/](https://ekd.global.bcs/) and [https://general.global.bcs/](https://general.global.bcs/) are using transparent authentication. Colleagues open the links in the browser and should be shown pages without any additional password prompts.

In order for this to work:


* in GMIB domains:
    * User's account should be in the correct domain (bcsprime for Moscow, bcsprimeuk for London etc)
    * On user's account in the GMIB domain employeeIndividualID field should be filled in with the Group AD account GUID. The GUID is shown in Lotus in the БКС.Юридическая структура (picture 1)

    
* in Group domains: 
    * User's global.bcs account must be in the correct OU. global.bcs/BCS/Users/IBB/NoAdmins for Moscow, global.bcs/BCS/Users/LON/NoAdmins for UK etc. If it is not the case, raise a Group Incident in Lotus in БД Инциденты (pictures 2)

    



Picture 1. GUID in Lotus

![](images/storage/image2021-10-29_10-44-6.png)



Picture 2. Group Incident

![](images/storage/image2021-10-29_10-44-40.png)







*****

[[category.storage-team]] 
[[category.confluence]] 
