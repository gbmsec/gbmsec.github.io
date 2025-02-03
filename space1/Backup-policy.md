



BCS GM





Backup Policy and Procedures

 

 

\[Version 1.8]

 

 

 

Table of Contents



About this document

Who should use this document?

Summary of changes

Chapter 1.  Procedures

1.1        System Administrator                                                                                              

1.2        Back Up Management                                                                                             

1.3        Device Management                                                                                       

1.4        Media Management                                                                                     

1.5        File Management                                                                                          

1.6        Error Reporting                                                                                                       

1.7        Error Recovery                                                                                                 

1.8        Agents                                                                                                           

1.9        Review of Back-up Tapes:                                                                               

1.10     Creation/Deletion of Backups according to Schedule:                                         

Chapter 2. Responsibility

2.1 Roles and Responsibilities                                                                                    

Appendix 1. Servers and resources

1.1       Section 1: Trading support servers:                                                                   

1.2       Section 2: Kondor+ department servers:                                                             

1.3       Section 3: Infrastructure department servers:                                                  

1.4       Section 4: DMA department servers:                                                                     

1.5       Section 5: QORT servers:                                                                               

1.6      Section 6:  HORIZON servers:                                                                            

1.7      Section 7:  Cyprus servers:                                                                             

1.8      Section 8:  UK servers:                                                                                         

1.9      Section 9:  Calypso servers:                                                                               

1.10    Section 10: Euclid servers:                                                                                               

1.11 Section 11:  Risk servers                                                                                          

1.11 Section 12:  ESB Fuse servers:                                                                              



Appendix 2 Media Management

Appendix 3 Backup request  template



About this documentThe unprecedented growth in data volumes has necessitated an efficient approach to data backup and recovery. This document is intended to provide details on the stipulations of data backup and retrieval operations to the client.

Who should use this document?This document should be used by:

BCS GM IT personnel responsible for the recovery and back up of all critical applications and

Electronic equipment.

 

Summary of changesThis section records the history of significant changes to this document.  Only the most significant changes are described here.

 



| Version | Date | Author | Description of change | 
| 1.0 | 07/05/2014 | Andrey Andreev | Created template | 
| 1.1 | 04/09/2014 | Andrey Andreev | Backup plan attached | 
| 1.2 | 20/03/2015 | Andrey Andreev | Media Management attached | 
| 1.3 | 04/04/2016 | Andrey Andreev | QORT backups attached | 
| 1.6 | 21/09/2016 | Maksim Vasilyev | Euroclid DB/App backup attached | 
| 1.7 | 01/01/2017 | Ilya Mirkovich | RISK DB backup attachedCalypso backup attached | 
| 1.8 | 11/12/2018 | Ilya Mirkovich | New sources attached, Tables changed | 

 

Where significant changes are made to this document, the version number will be incremented by 1.0.  

Where changes are made for clarity and reading ease only and no change is made to the meaning or intention of this document, the version number will be increased by 0.1.

Chapter 1.  Procedures1.1             System AdministratorThe System administrator should ensure that backups of software on the servers are performed,

and that the tapes are properly stored and locked. Where possible, the system administrator should backup all affected system/application software

before system upgrades or maintenance occurs.

1.2            Back Up ManagementThe servers (see Appendix 1) contain the critical data/applications for the BCS GM

and the safety of that data depends upon the backup tasks being performed on schedule. The

operation of backup tasks requires a high level of discipline. Backup management software (e.g.

Symantec Backup Exec) is used for automatically scheduling backup tasks. Backup management

software will automate all aspects of the backup strategy.

Back up policy should be applicable for all critical IT assets including ( e.g. File server, Mail

Server, Database server, Lotus Replication server, Trading Servers, BO/MO servers etc).



1.3            Device ManagementBackup software will recognize and manage all the devices that will be used at the BCS GM for taking backups. In case multiple drives are used, backup software will have the ability to direct the data to the appropriate device and media.



1.4            Media Management Media management provided in appendix 2. Media management document will include tape sets of daily, weekly and monthly backups, which will rotated for overwriting



Some data will keep about 7 years and stored on tapes without overwriting.





 The backup management software will keep track of the media involved, labelling of each unit

and loading of specific media while restoration.



1.5            File ManagementBackup management tool will track the status of each file on the storage system. It will maintain a

database that includes information on when each file was backed up, what tape it is on, and the

like. This information is critical for file restorations. If a user accidentally deletes a file, it can be

tracked using the backup tool database. It will also contain the information as to which tape

contains the latest version. In case of file being corrupted, the older version can also be restored.

1.6            Error ReportingThis is required to make sure that the backup was successful. The error reports can be printed or

sent through E-Mail. The report will indicate the status of backup with the detailed report on any

error.

1.7            Error RecoveryThere must be a mechanism to overcome the errors. For example the backup tool can be used to

schedule the backup of the missed files at the end of the run.

Error recovery policy can consists many mechanisms of automated actions, configured in the backup software.

The backup software using agents which have to installed on targeted systems and all issues tracked by agents and tasks re-run automatically or manual.



1.8            AgentsRemote agents (e.g. Oracle, Lotus, Active Directory, Windows servers) are deployed on the

servers that need to be backed up. Backup tool supports agents on multiple platforms so that

multiple platforms can be backed up with the same management tool.

1.9            Review of Back-up Tapes:The backup operator should inspect all backup tapes on a monthly basis by making a re-storing

testing exercise.  

1.10            Creation/Deletion of Backups according to Schedule:System administrators should ensure that the daily/monthly backups are executed according to the schedule and that the backup tapes are deleted according to the schedule.  



Following server needs to be backed up, see Appendix 1

 Chapter 2. Responsibility



2.1 Roles and Responsibilities
* Ensuring that the backup procedures are implemented is the responsibility of the system
* Ensuring that the necessary re-store of data is performed and backup tapes are checked properly is the responsibility of the backup operator.
* Enforcement of these procedures is the responsibility of the CIO GMIB
* Ensuring that the Systems and backup operator performs their tasks are the responsibility of the Head of Infrastructure of BCS GMIB





Note: This policy document should be reviewed whenever there are changes in the

organisations computer system.



Appendix 1. Servers and resources.



1.1  Section 1: Trading support servers:



|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| cifs_svn.bcsprime.local | \\cifs_svn.bcsprime.local\TS_Archive\ | 2.8Tb | +70 Gb/month | Saturday | 21:00 | FULL | 7 years |  | Alexander Efimov | 
| cifs_svn.bcsprime.local | \\cifs_svn.bcsprime.local\TS_Backup\FullBackup | 19 Gb | +1 Gb/month (old archives will removed) | Saturday | 21:00 | FULL | 1 month |  | Alexander Efimov | 
| cifs_svn.bcsprime.local | \\cifs_svn.bcsprime.local\TS_Backup\Configuration files\ | 1.9 GB | Old archives will removed, size doesn’t change | Saturday | 21:00 | FULL | 1 month |  | Alexander Efimov | 
| cifs_svn.bcsprime.local | \\cifs_svn.bcsprime.local\TS_Backup\Logs\ | 980 Gb | Old archives will removed, size doesn’t change | Saturday | 21:00 | FULL | 7 years |  | Alexander Efimov | 



All information must be kept for a minimum of seven years.

We will keep monthly backups without overwriting at least 7 years

1.2  Section 2: Kondor+ department servers:



|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| AG-KONDORDB | Kplus, KplusArchive, KplusVersion, Ksp, Ksystem, Kustom, WA, insight | 400 Gb |  ** **  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, Sunday | 04:00 | DIFF,FULL |  7 Years | confidential | Mikhail Bashkov | 
| AG-LRADIUS | DB: Rubica, BloombergFI, Dealing, MQueues, Monitoring, TradeEcho, KondorDB. LSE, Factor, Micex | 540Gb |  ** **  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, Sunday | 04:00 | DIFF,FULL |  7 Years | confidential | Mikhail Bashkov | 
| l-kondor-db | /dump/archive/dump | 85 Gb500 Mb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday | 05:00 | FULL |  7 Years | confidential | Mikhail Bashkov | 
| L-QEXPORT | VM | 220Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday | 04:00 | DIFF,FULL |  14 Days |  | Mikhail Bashkov | 
| M-DEALTRACKER | VM | 100 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday | 04:0022:00 | DIFF,FULL | 14 Days |   | Mikhail Bashkov | 
| M-KONDOR-TERM | VM | 260 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday | 22:00 | DIFF,FULL | 14 Days |   | Mikhail Bashkov | 
| M-QEXPORT | VM | 220 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday | 22:00 | DIFF,FULL | 14 Days |   | Mikhail Bashkov | 
| M-Radius | VM | 1 TB1000 Mb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday | 04:00 | DIFF,FULL | 14 Days | confidential | Mikhail Bashkov | 
| M-TRADIUS | VM | 390 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday | 22:00 | DIFF,FULL | 14 Days |  | Mikhail Bashkov | 



1.3  Section 3: Infrastructure department servers:



|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| Analityca-SQL | VM | 292 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days | confidential | Database Team | 
| Autosave01 | VM | 132 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days |  | Server Team | 
| BizTalk | VM | 45 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days | Confidential | Server Team | 
| Confluence | VM | 65 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days |  | Server Team | 
| Consultant | VM | 200 Gb              |  | Saturday | 22:00 | DIFF,FULL | 7 days |  | Server Team | 
| dba02 | VM | 200 Gb              |  | Saturday | 22:00 | DIFF,FULL | 14 days |  | Database Team | 
| DC01.bcs-prime.local | VM | 70 Gb              |  | Tuesday, Thursday, Saturday, | 22:00 | DIFF,FULL | 7 days | Confidential | Network Support Team | 
| DC02.bcs-prime.local | VM | 100 Gb              |  | Tuesday, Thursday, Saturday, | 22:00 | DIFF,FULL | 7 days | Confidential | Network Support Team | 
| DC05 | VM, AD | 66 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days | Confidential | Server Team | 
| dcix-teamdev02 | VM | 60 Gb              |  | Saturday | 22:00 | FULL | 14 days |  | Database Team | 
| dcix-vcenter01 | VM | 208 Gb              | 1Gb | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days |  | Server Team | 
| DCIX-vHLB01 | VM | 16 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 03:00 | DIFF,FULL | 14 days |  | Server Team | 
| DCIX-vHLB02 | VM | 16 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 03:00 | DIFF,FULL | 14 days |  | Server Team | 
| DCIX-vHUAG01 | VM | 20 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 03:00 | DIFF,FULL | 14 days |  | Server Team | 
| DCIX-VHVCS01 | VM | 60 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 03:00 | DIFF,FULL | 14 days |  | Server Team | 
| DCIX-VHVCS02 | VM | 60 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 03:00 | DIFF,FULL | 14 days |  | Server Team | 
| dcld4-git.bcsprime.local    | VM | 210Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days |  | Server Team | 
| DCM1-DC01 | VM | 100 Gb              |  | Monday, Wednesday, Friday, Saturday | 22:00 | DIFF,FULL | 14 days | Confidential | Server Team | 
| DCM1-GOODTest  | VM | 100 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days |  | Server Team | 
| DCM1-Safenet | VM | 100 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days |  | Server Team | 
| DCM1-SP-APP1 | VM | 200 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days |  | Aleksey Polezhaev | 
| DCM1-SP-DB1 | VM | 270 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days |  | Aleksey Polezhaev | 
| DCM1-SPS-DEV1 | VM | 120 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days |  | Aleksey Polezhaev | 
| DCM1-SP-WEB1 | VM` | 200 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days |  | Aleksey Polezhaev | 
| dcm1-vcenter         | VM | 290 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 04:00 | DIFF,FULL | 14 days |  | Server Team | 
| dspcolo-zabbix | /var/lib/mysql/zabbix, /var/lib/mysql/mysql | 100 Gb |  | Saturday | 10:00 | FULL | 30 days |  | Server Team | 
| Jabber | VM | 16 Gb              |  | Saturday | 22:00 | FULL | 14 days |  | Server Team | 
| JIRA | /opt/atlassian/jira/logs/access\*                | 30 Gb | 4 Gb | Saturday | 22:00 | FULL | 7 years |  | Nikolay Lupin | 
| Lansweeper | VM | 180 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 14 days |  | Server Team | 
| OEM | VM | 400 Gb              |  | Saturday | 20:00 | FULL | 14 days |  | Database team | 
| PMIRA-DC01 | VM | 100 Gb              |  | Monday,  Wednesday,  Friday, Saturday | 22:00 | DIFF,FULL | 14 days | Confidential | Server Team | 
| pmira-kav | VM | 50 Gb              |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | 22:00 | DIFF,FULL | 7 days |  | Server Team | 

 

 

1.4  Section 4: DMA department servers:



|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| Dcix-fix01 | /var/app, /var/app_backup | 2 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday | 00:35 | FULL | 1 Month | Confidential | Prime_DMA | 
| Dcix-fix02 | /var/app, /var/app_backup | 14 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday,Sunday | 23:30 | FULL | 1 Month | Confidential | Prime_DMA | 
| Dcix-fix03 | /var/app, /var/app_backup | 36 Gb | 2 Gb | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday,Sunday | 23:30 | FULL | 1 Month | Confidential | Prime_DMA | 
| Dcix-fix04 | /var/app, /var/app_backup | 22 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday,Sunday | 00:35 | FULL | 1 Month | Confidential | Prime_DMA | 
| Dcm1-fix02 | /var/app, /var/app_backup | 30 Gb | 2 Gb | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday,Sunday | 23:30 | FULL | 1 Month | Confidential | Prime_DMA | 
| Dcm1-fix05             | /var/app, /var/app_backup | 44 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday,Sunday | 00:45 | Full | 1 Month | Confidential | Prime_DMA | 
| DMAbackup | /opt/backups, /opt/backups2 | 80 Gb |  | Friday | 23:00 | FULL | 7 Years | Confidential | Prime_DMA | 
| Dmabackup-mos | /opt/backup | 515 Gb |  | Friday | 23:00 | FULL | 7 Years | Confidential | Prime_DMA | 
| dsp-horizon | /home/horizon/HMM-PROD | 123 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday,Sunday | 05:00 | FULL | 14 Days | Confidential | Prime_DMA | 
| horizon-uat | /home/horizon/HMM-UAT | 39 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday,Sunday | 06:00 | FULL | 14 Days | Confidential | Prime_DMA | 
| LSE-fix01 | /var/app, /var/app_backup | 8.3 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday,Sunday | 23:30 | FULL | 1 Month | Confidential | Prime_DMA | 
| M1colo-fix01 | /var/app, /var/app_backup | 2.4 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday,Sunday | 00:35 | FULL | 1 Month | Confidential | Prime_DMA | 
| M1colo-fix02 | /var/app, /var/app_backup | 14 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday,Sunday | 05:00 | FULL | 1 Month | Confidential | Prime_DMA | 
| M1colo-fix03 | /var/app, /var/app_backup | 19 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday,Sunday | 23:30 | FULL | 1 Month | Confidential | Prime_DMA | 

 

1.5   Section 5: QORT servers: 

|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| DCIX-QORTAPPCY | d:\!_ARHIV\, d:\FTP_ROOT\ | 870 Gb | 10 Gb | Saturday every 6 month | 22:00 | FULL | 7 Years | Confidential | QORT Support team | 
| DCM1-DB-QORT-1 | E:\KondorToQortService\, D:\KSPToQortService\ | 2.1 Gb | 0.1 Gb | Saturday every 6 month | 22:00 | FULL | 7 Years | Confidential | QORT Support team | 
| QORTDBCY | \\qortdbcys\Backup\qortrepldbcy                |                 740 Gb with 2 weeks stored files         | 10 Gb | Full on every Sunday 4 a.m., Diff in every  other days at 3.50, Logs every 30 minutes | Full 1.5 hours, Diff 5 minutes, less than minute fo logs | DIFF,FULL | 2 weeks | Confidential | QORT Support team | 
| qortrepldbcy | \\qortdbcys\Backup\qortrepldbcy                |                 599 Gb for 2 weeks files stored | 10 Gb | Full on every Sunday 4 a.m., Diff in every  other days at 3.50                |  | DIFF,FULL | 2 weeks | Confidential | QORT Support team | 

1.6 Section 6:  HORIZON servers:



|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  |  | 
| HorizonPROD | /home/horizon | 66 Gb | 8 Gb | Weekly | Sunday 05:00 | FULL | 3 Weeks | Confidential | QORT Support team |  | 
| HorizonUAT | /home/horizon | 11 Gb |  | Weekly | Sunday 03:50 | DIFF | 3 Weeks | Confidential | QORT Support team |  | 

 

1.6  Section 7:  Cyprus servers:





|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| cyp-cas01 | VM | 70 Gb |  | Monday, Wednesday, Friday, Saturday | 21:00 | DIFF,FULL |  | Confidential | Server Team |  | 
| cyp-cas02 | VM | 70 Gb |  | Tuesday, Thursday, Saturday | 21:00 | DIFF,FULL |  | Confidential | Server Team |  | 
| CYP-DC01 | VM | 50 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, | 23:00 | DIFF,FULL | 7 Days | Confidential | Server Team |  | 
| CYP-DC02 | VM | 50 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, | 23:00 | DIFF,FULL | 7 Days | Confidential | Server Team |  | 
| CYP-FS | E: | 1.3 Tb |  | Monday, Tuesday, Wednesday, Thusday, Friday | 23:0021:00 | DIFF,FULL | 7 Years | Confidential | Server Team |  | 
| cyp-mbx01 | VM | 560 Gb |  | Monday, Wednesday, Friday, Saturday | 21:00 | DIFF,FULL |  | Confidential | Server Team |  | 
| cyp-mbx02 | VM | 570 Gb |  | Tuesday, Thursday, Saturday | 21:00 | DIFF,FULL |  | Confidential | Server Team |  | 
| cyp-mx02 | VM | 500 Gb |  | Monday, Wednesday, Saturday | 00:00 | DIFF,FULL | 7 Years | Confidential | Server Team |  | 
| cyp-mx04 | VM | 500 Gb |  | Monday, Wednesday, Saturday | 00:00 | DIFF,FULL | 7 Years | Confidential | Server Team |  | 

 1.8 Section 8:  UK servers:

|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  |  | 
| DCIX-DC01 | VM | 65 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday | 22:00 | DIFF,FULL | 14 days | Confidential | Server Team |  | 
| DCIX-DC02 | VM | 65 Gb |  | Monday, Tuesday, Wednesday, Thursday, Friday, Saturday | 22:00 | DIFF,FULL | 14 days | Confidential | Server Team |  | 
| DCIX-FS01 | C:S: | 1.1 Tb |  | Monday, Tuesday, Wednesday, Thursday, Friday | 23:00 | DIFF,FULL | 7 Years | Confidential | Server Team |  | 

 1.9 Section 9:  Calypso servers:



|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| CALYPSODB | CALYPSO | 1 Tb | 100 Gb | Weekly | 02:00 | FULL | 1 Month | Confidential | Alexey Isaev |  | 
| CALYPSODB | CALYPSO | 1 Tb | 100 Gb | Monthly | 02:00 | FULL | Never |  | Alexey Isaev |  | 
| CALYPSODB | CALYPSO | 200 Gb | 30 Gb | Daily | 04:00 | DIFF | 1 Month | Confidential | Alexey Isaev | 
| CALYPSODB | /u01/app/rman_backup | 4.7 Tb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, Sunday | 06:00, 04:00 | DIFF,FULL | 7 years | Confidential | Database Team | 
| capp01 | VM | 200 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, Sunday | 01:00 | DIFF,FULL | 14 Days | Confidential | Database Team | 
| capp02 | VM | 200 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, Sunday | 01:00 | DIFF,FULL | 14 Days |  | Database Team | 
| CREPORTS | VM | 30 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, Sunday | 01:00 | DIFF,FULL | 14 Days |  | Database Team | 
| dcld4-dfs01 | \\bcsprime.local\Calypso\Prod | 400 Gb | 50Gb | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, Sunday | 00:01, 03:00 | DIFF,FULL | 7 years | Confidential | Server Team | 
| DEV-CAPP01 | VM | 500 Gb |  | Saturday | 22:00 | FULL | 14 days |  | Database Team | 

1.10 Section 10:  Euclid servers:





|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| DCM1-CYEUAPP | VM | 59 Gb |  | Daily | 01:00 | DIFF,FULL | 7 Days | Confidential | Andrey Yushin |  | 
| DCM1-CYEUDB | VM | 55 Gb |  | Daily | 01:00 | DIFF,FULL | 7 Days | Confidential | Andrey Yushin |  | 
| DCM1-UKEUAPP | VM | 55 Gb |  | Daily | 01:00 | DIFF,FULL | 7 Days | Confidential | Andrey Yushin |  | 
| DCM1-UKEUDB | VM | 55 Gb |  | Daily | 01:00 | DIFF,FULL | 7 Days | Confidential | Andrey Yushin |  | 

1.11 Section 11:  Risk servers:





|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| EXP1-RISK | VM | 100 Gb |  | Sunday | 06:00 | FULL | 7 Days |  | David Khutinaev |  | 
| RiskRoom-Archive | All |  |  | Mounthly | 00:00 | DIFF,FULL | FULL 7 years | Confidential | Ruslan Gizatullin |  | 



1.11 Section 12:  ESB Fuse servers:



|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| dcix-fuseproduk01 | VM | 260 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, Sunday | 01:00 | DIFF,FULL | 14 days |  | ESB Support |  | 
| dcix-fuseproduk02 | VM | 100 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, Sunday | 01:00 | DIFF,FULL | 14 days |  | ESB Support | 
| dcix-fuseproduk03 | VM | 100 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, Sunday | 01:00 | DIFF,FULL | 14 days |  | ESB Support | 
| dcix-rabbituk | VM | 50 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, Sunday | 01:00 | DIFF,FULL | 14 days |  | ESB Support | 
| FUSEDBUK | QUARTZ,master,quickfix,ESB_ARC_MSG,msdb,ESB_MQSTORE | 96 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday, Sunday | 03:00, 02:00 | DIFF,FULL | 14 days |  | ESB Support | 



1.11 Section 13:  WebPortal GMIB:



|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| webportal01 | VM | 150 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 04:00 | FULL | 14 days | Confidential | Database Team |  | 
| webportal02 | VM | 400 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 04:00 | FULL | Weekly | Confidential | Database Team |  | 



1.11 Section 14: Skype for Bussines servers:





|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| dcix-s4b0front02 | VM | 60 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 02:00 | DIFF,FULL | 14 days |  | Server Team |  | 
| dcix-s4b-dc01 | VM | 60 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 02:30 | DIFF,FULL | 14 days |  | Server Team |  | 
| dcix-s4b-dc02 | VM | 60 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 02:30 | DIFF,FULL | 14 days |  | Server Team |  | 
| dcix-s4b-edge | VM | 60 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 02:30 | DIFF,FULL | 14 days |  | Server Team |  | 
| dcix-s4b-fim | VM | 60 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 02:30 | DIFF,FULL | 14 days |  | Server Team |  | 
| dcix-s4b-front01 | VM | 60 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 02:30 | DIFF,FULL | 14 days |  | Server Team |  | 
| dcix-s4b-Perchat | VM | 100 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 02:30 | DIFF,FULL | Weekly |  | Server Team |  | 

1.11 Section 15: Development servers:





|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| dcm1-dev01.bcsprime.local | D:\SvnRepositories, D:\Bonobo.Git.Server\, D:\Nuget.Server | 3.5 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 04:00 | DIFF,FULL | 14 days |  | Oleg Abakumov |  | 
| DCM1-MO-BO-UAT.bcsprime.local | В:\Repositories | 5.04 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 04:00 | DIFF,FULL | 14 days |  | Oleg Abakumov |  | 



1.11 Section 14: Other servers:





|  **Server Name**  |  **Source**  |  ** **  **Size**  |  ** **  **Presumptive Growth Month**  |  **Day of Week**  |  **Time to Run**  |  **Backup Type**  |  **Ability to Overwrite Data**  |  **Level of Confidentiality**  |  **Responsible Person**  | 
| BCSDB-01.bcsprime.local | C:\Program Files (x86)\stunnel, C:\Work, D:\Quik | 1 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 02:00 | DIFF,FULL | 14 days |  | Database Team |  | 
| Salesforce system backup | System sends backup archives to salesforce administrator, backup archives placed in \\dcix-storserv01\Salesforce | 40 Gb | 150mb | Wednesday | All day | FULL | 1 year | confidential | Andrey Lebedev |  | 
| dcm1-quantVM | VM | 400 Gb |  | Monday, Tuesday, Wednesday, Thusday, Friday, Saturday | 04:00 | DIFF,FULL | 7 days |  | QuantDesk |  | 

Appendix 2 Media Management





|  **Media Stack Name**  |  **Backup type**  |  **Description**  | 
| Calypso | Daily | Calypso development data backup | 
| Weekly | 
| DFS Month | Monthly | File storage data backup | 
| DFS Year | Yearly | File storage yearly backup | 
| DMA | Daily | DMA hardware servers backup | 
| Weekly | 
| Exchange | Yearly | IB Exchange mail data backup | 
| QUIK | Weekly | Trading support and QUIK servers backup | 
| Monthly | 
| Infrastructure | Daily | Infrastructure department servers and VM backup | 
| Weekly | 
| Monthly | 
| Cyprus | Monthly | File storage data backup | 
| United Kingdom | Monthly | File storage data backup | 
| Euclid | Daily | Euclid DB and application backup | 
| Weekly | 

 

Appendix 3 Backup request template

 

 



|  **Name**  |  _Person who requesting backup_  |  **tel:**  |  _number_  |  |  |  |  |  |  | 
|  **Dept**  |  _Department name_  |  |  |  |  |  |  |  |  | 
|  _Service name_  |  **Information**  |  **Schedule**  |  **Ability to overwrite data on the disk after:**  |  **Level of confidentiality**  |  **Responsible person**  | 
|  **Size**  |  **Presumptive growth month**  |  **Day of the week**  |  **Time to run**  |  **Backup type**  | 
|  **Server name**  |  **Target directory**  |  |  |  |  |  |  |  |  | 
|  |   |  |  |  |  |  |   |   |  | 
|  |  |  |  |  |  |  |  |  |  |  | 

 

 



*****

[[category.storage-team]] 
[[category.confluence]] 
