
### Cyprus audits folder \\cyp-fs\public\Common\Internal Audit 2020\IT\


| BCS Cyprus internal IT audit for 2022 year (Wizberry) |  | 

 | Findings:-Lack of periodic review of users’ access rights. The process doesn't exist neither on paper nor in fact.  -Disorder in access management documents. Documents doesn't reflect the current access management arrangements in place. | [SD-357251 BCS IB JIRA](https:///browse/SD-357251)

[SD-357250 BCS IB JIRA](https:///browse/SD-357250)

 | 
|  --- |  --- |  --- |  --- |  --- | 
| Audit | administrator | Audit report | Findings | Jira tasks to resolve the remark | 
|  **MAZARS UK Audit for 2023 ( march 24)**  |  |  | Findings:
1. We inspected 100% of the accounts identified as having privileged access to the MS Dynamics and noted one (1) business user (Elena Basko - Finance Change manager) granted privileged access (system administrator role) to the application.
1. For the sampled change requests below, we could not ascertain whether the changes requested were appropriately tested and approved before moving to production environment due to the lack of adequate UAT and approvals documentation from change requestor, approver through to implementation:




    1. Sample Change (Calypso) - ID 3066, MSD 365 - Finance & VM enhancement

    
1. We noted that the parameter for password history (i.e number of passwords remembers) was not set on Calypso.



In addition, we noted that the BCS Cyber Crime Prevention Policy states that the password policy must be enforced to ensure minimum password length and complexity requirements are met for all user access credentials, however, for the sampled new user account created for Artem Zikarov (Contractor), we noted that no password parameter requirements had been set for this user's profile.


1. For the sampled access modification for user Ksenia Starodumova (Office Administrator (UK), we could not ascertain if the user access modification had been appropriately requested, approved and if access granted in the system was appropriate due to lack of formal access request documentation for the access granted to user profile
1.  **MS Dynamics / ESB /AD:** 

We noted that a formal user access review was not performed and/or documented for MS Dynamics, ESB and Active Directory applications.



 **Calypso:** 

For Calypso, an automated report has been created which identifies any permission changes in the previous day. We noted that evidence of review performed did not include approval workflows or email correspondence between the personnel involved and any action points noted from review following receipt of the system report and hence we concluded that the control is not designed and implemented appropriately.
1.  **Change Management and Back-up policy** 

We noted from testing that formally documented and approved versions of the Change management and Back-up policies were not in place to ensure that the processes being followed for change and back-up management are consistent across the organization and in line with the management's intent.



 | 1) Create Finadmin role - IN PROGRESS

    Remove system administrator role  from E.Basko - TO DO

    Click HR  - add MSD Service  for future access requests  - DONE

      SYNC Click HR UK vs MSD  - DONE

2) NO actions

    

3) Finding #2 is about change made in MSD environment. Locally we don't conduct testing, all  development and testing is outsources and validated by the business user.

Appropriate change in Jira contains Word documents that contains all business user approvals done in the email. Everything is inside embedded word file.

So,  all approvals are linked into change in Jira.



3) [SD-359341 BCS IB JIRA](https:///browse/SD-359341)   DONE

4) Communication with UK Staff  with instructions to follow IT Processes .DONE

5)  Access rights review   TO DOIt was mentioned to audit several times that ESB is system software and doesn't have any user interface and registered users it. For ESB users review is not applicable. | 
|  **BCS Cyprus ROPA 2023**  |  | audit report 

management response 

 |  **Findings:** - **the Organization does not apply password protection to personal data transferred electronically, either internally (to other departments of the Organization) or to external parties (vendors/processors).**  **-upon the resignation of an employee, his/her corporate email address remains active and can be accessed by the IT department. During this time, the whole history of the mailbox is accessible.**  **-the Company has removed the CCTV labelling from the main entrance of the office floor and no other labelling exists to inform the data subjects that the area is monitored with CCTV technology.**  **-Data store Retention period should be established as long as 8 years in BCS CY systems**  | [SD-357743 BCS IB JIRA](https:///browse/SD-357743)

[SD-357742 BCS IB JIRA](https:///browse/SD-357742)

[SD-354112 BCS IB JIRA](https:///browse/SD-354112)

[SD-357256 BCS IB JIRA](https:///browse/SD-357256)

 | 
|  **BCS Cyprus Wizberry ICT security audit 2024**  |  | audit report 

management responses 

 | Findings:<ul><li>lack of security awareness trainings for employees and IT staff</li><li>absence of ICT strategy, Third party relationship policy. Continual service improvement document needs improvements</li><li>absence of ICT and security risk assessment</li><li>absence of Business impact Assessment</li><li>Information security framework provided, needs improvements </li><li>lack of formal vulnerability assessment policy and procedure</li><li>lack of formal Backup and archive policy in place</li><li>Business continuity and Disaster recovery plans are in place, but need improvements based on BIA, which is also absent. </li></ul> |  | 





*****

[[category.storage-team]] 
[[category.confluence]] 
