





|  

 | 
|  

 | 
| 

 | 
|  **TBA**  | 
|  **TBA**  | 
|  --- | 
|  --- | 
|  --- | 
|  --- | 
|  --- | 
|  

 | 
|  

 | 
| 

 | 
|  **TBA**  | 
|  **TBA**  | 











|  **Document Title**  | Software Development Life Cycle (SDLC) Policy | 
|  **Applicability and objectives**  |   This Policy applies to all application projects, both new applications and upgrades of existing applications, under the purview of the Chief Information Officer (CIO), irrespective of hosting location. This document is for use by all employees of BCS Global Markets | 
|  **Department**  | IT | 
|  **Document **  **Owner**  | Maksim Kevish | 
|  **Approved by**  | Control and Oversight Committee | 
|  **Date of approval**  |  _November 2021_  | 
|  **Approval list (if applicable)**  |  **Name**  |  **Signature**  |  **Date**  | 
|  **Process Manager**  | Aleksey Dorogov |  |  | 
|  **CIO**  | Viktor Frolov |  |  | 
|  |  |  |  | 
|  **Effective Date**  |  _Immediate_  |  **Review Date**  | November 2021 | 
|  **Revision Cycle**  |  _Annually_  |  **Document access**  | Internal | 
|  **_Version No_**  |  **_Date_**  |  **_Reviewed by_**  |  **_Notes_**  | 
| 1 | 08/11/2021 | Maksim Kevish | First version of the document | 
|  |  |  |  | 

 **Terms and definitions** 

|  **Term**  |  **Abbreviation**  |  **Definition / Explanation**  | 
| Software Development Life Cycle | SDLC | Software production  **PROCESS**  | 
| Functional Domain | FD | A separate area of the architectural landscape (including all layers of architecture) to develop support for a product/group of similar products or processes. It is a tool for managing the complexity and decomposition of the architectural landscape. FD allows you: group goals and objectives; define teams; optimally manage tasks  | 
| Conceptual Architecture of  Functional Domain | CAFD |  | 
| Product |  | A product is a set of services that provide satisfaction of certain clients needs. (At the same time, clients are both  _internal_  and  _external_ ) | 
| Product Vision |  | Answers questions: what? for whom? and why? we doConsists of:<ul><li>description of the product idea</li><li>description of the values that the product brings</li><li>description of the target audience of the product</li><li>description of strengths and weaknesses, opportunities and threats</li></ul> | 
| Product backlog |  | A prioritized list of all known features or outstanding work necessary to bring the product to life. This may include customer/ user needs, technological, functional and non-functional requirements | 
| Feature |  | An element of the backlog, the result of the implementation of the solution, the functionality of a specific product or group of stories that can satisfy one or more interrelated needs of the client or other AS or services. The feature is not an object of release management, that is, it is not included in the release. Improvements to the program code implemented in the release and implemented on the industrial environment as part of the distribution are described in the stories that the feature is decomposed into.The feature must match the following properties:- focuses on the product, i.e. answers the question "WHAT needs to be done?" rather than "HOW should I do it?"- formulated as a specific solution or product functionality- implemented within a single product- developed mainly by one team related to the implementation of a relevant product/project- has specific acceptance criteria - aimed at a specific external or internal user- decomposes on story | 
| Story |  | The main element of decomposition of product backlog element, which contains a brief formulation of the system function from the point of view of the user (client) the system. The wording expresses the atomic need of the user, which carries value for him. Stories are designed to work on creating new program code or changing existing program code, for example refactoring.The following changes can be implemented within the story:- an independent part of the functionality of the feature- functionality that brings value to the business and is related to the goals of the customer- technical changes | 
| Set of Technical Tools | STT |  | 
| User Acceptance Testing | UAT |  | 
| Change Request / Small Request | CR / SR |  | 

 **General regulation** 
## Process goal
Design, development and implementation of technological changes in the shortest possible time and with proper quality


## How the goal is achieved

1. Description and implementation of an end-to-end software production process covering all disciplines of software production from needs analysis to solution installation, including a description of the roles and responsibilities of process participants and process artifacts
1. Building a process management system, quality control and continuous improvement of process efficiency based on measurable indicators


## The process based on
SDLC process is based on the practices of design thinking, the principles of architectural unity, the provisions and principles of the AGILE manifesto and DevOps practices

 **Process Description** 
## Participants
The following roles are allocated within the process:



| 1 | Product owner ( **customer** ) | 
| 2 |  **Сustomer**  representative | 
| 3 | Process Owner | 
| 4 | Leader/Head of the Functional Domain (FD) | 
| 5 | Business Analyst | 
| 6 | System Analyst | 
| 7 | Architect | 
| 8 | Designer | 
| 9 | Developer | 
| 10 | Tester | 
| 11 | DevOps Engineer | 
| 12 | Cybersecurity Expert | 
| 13 | Infrastructure Engineer | 
| 14 | Support Engineer | 
| 15 | Release Manager | 
| 16 | Delivery manager\* | 

\*- Now this role is performed by a project manager PM

 **Life cycle of process objects** 
1. 
###  Feature/CR/SR/TechDebt/Bug

    1.1. Diagram

    ![](images/storage/LC Feature.png)

    1.2. Tabular description of the life cycle diagram (Feature/CR and etc.)


|  **№**  |  **Life Cycle stage**  |  **Description**  | 
| 1 | Idea / Planning | Formulation of need, inclusion in product backlog, planning of the desired implementation date | 
| 2 | Decomposition | Decomposition of backlog element on story, ensuring the readiness of the story to be taken into work | 
| 3 | Implementation | Analysis, detailed design the changeable part of the business process, implementation architectural design at the application/integration level, definition requirements for specific AS/Services, coding solution, passing the full cycle of necessary testing | 
| 4 | Acceptance | Conducting acceptance tests on features/story for compliance with task being solved and requirements of interested parties | 
| 5 | E2E testing (optional stage) | Testing as part of the business process | 
| 6 | Inclusion in release | The elements that have been successfully accepted are included in release which implementation is planned | 
| 7 | Testing and acceptance within the final distribution | Testing and acceptance as part of the final distribution. If the distribution kit contains only one feature and has not changed after the "Acceptance" stage, then the stage can be limited only to installation testing | 
| 8 | Implementation - Pilot/Trial operation (optional stage) | Deployment as part of final distribution kit to industrial stands for trial/pilot operation | 
| 9 | Implementation - Production operation | The feature /CR/SR has been put into production operation and replicated to target number of users | 




1. 
### Release

    2.1. Diagram

    ![](images/storage/LC Release.png)

    2.2. Tabular description of the life cycle diagram (Release) 


|  **№**  |  **Life Cycle stage**  |  **Description**  |  **Comment**  | 
| 1 | Planning and implementation | Planning and implementation of release composition | The date of the next release has been determined, the composition of the release for testing has been fixed | 
| 2 | Testing and release acceptance | Regression, load and installation testing of the release distribution | The composition of the release for implementation has been fixed | 
| 3 | Preparation for implementation | Preparation of implementation order | The implementation order is ready and approved | 
| 4 | Implemented | The release has been put into operation | The release has been put into pilot/trial or production operation | 





 **Process diagram** 
1. 
## Process "Implementing the element of product backlog"

## 1.1. Process diagram

    ![](images/storage/SDLC-Feature.PNG)

## 1.2.  Tabular description of process diagram


|  **№**  |  **Step's name**  |  **Step description**  |  **Executor**  |  **Input**  |  **Output**  |  **Quality gate**  |  **Responsible for Quality Gate**  | 
| 1 | High-level planning | Inclusion related teams, planning desired implementation date.  Customer/Сustomer representative or/and  team leaders, based on CAFD and accumulated knowledge, determine the adjacent teams whose help will be required to implement the feature and send CR/SR to these teams in JIRA and indicating desired implementation date.  Team that has received a top-level description of the task analyzes the possibility of implementation in the desired time frame and confirms them or offers an alternative | Product owner ( **customer** ) / Сustomer representativeTeam LeadersBusiness Analyst | Product backlogCAFDDesired implementation date | List of  **_Features_**  |  |  | 
| 2 | Analysis | Create detailed design of the changeable part of the business process (business service scenario). Together with Team, related parties and stakeholders, the Product owner forms and describes business requirements of feature, designs the target scenario (new or changes in the existing one) and determines the acceptance criteria, after which he checks the results with the participants. In the future, the results can be refined as the stories are implemented | Business Analyst |  **_Feature_** CR with the desired release numberProduct VisionCAFDProcess Description |  **_Feature_** Process Description (To Be) |  **Mandatory** :
    1. Business requirements (Non Functional and functional requirements) for REQ (SR) or EPIC 
    1. Acceptance criteria's including testing strategy
    1. Process Description in Business Studio

     **Optional** :
    1.  Indicators for business monitoring are defined

     | Product owner (customer) / Сustomer representativeTeam Leaders | 
| 3 | Designing | Detailed architectural design at the application and/or integration level. The team members, together with the subcontractors and the AS/Service architect/system analyst, design an architectural solution. The results are entered into service architecture and validated. In the future, the results can be refined as the story is implemented. If during this step the need to change the CAFD is revealed, the team engages an architect | ArchitectSystem AnalystDevelopment Team |  **_Feature_** Process Description (To Be)CAFD | AS/Service architecture (Detailed architecture) |  **Mandatory:** 
    1. КА ФО Architecture validation. Arch com if needed  to modify КА ФО
    1. Capacity check and HW control
    1. CISO control
    1. Licensing requirements for software components

     | Team LeadersCybersecurity ExpertInfrastructure Engineer | 
| 4 | Decomposition and preparation for implementation | Ensuring that story is ready to be taken into work. The customer, together with team, decomposes the entire feature into stories that can be implemented in a sprint. Further, as part of regular grooming, stories are prioritized, analyzed and evaluated. The team determines whether there is enough data to implement the story and, if necessary, conducts additional work | Product owner ( **customer** ) / Сustomer representativeTeam LeadersBusiness Analyst |  **_Feature _** Process Description (To Be)AS/Service architecture (Detailed architecture) | Story/s | Release has been created | Release Manager | 
| 5 | Story implementation (cycle) | After planning sprint, for each of planned stories, team performs all the necessary tasks for its implementation (additional analysis, design, coding of solution, passing full cycle of necessary testing) | Development Team | Story/sAS/Service architecture (Detailed architecture) | DistributiveA set of scripts and/or configuration filesTesting reports ST, IFT, LT |  | Release Manager | 
| 6 | Testing | If a release is planned based on results of sprint, then the set of release candidate is determined and fixed. Based on it, UAT is carried out. In case of successfully passed UAT, the implementation is initiated[[Software Testing Procedure|Software-Testing-Procedure]] | Product owner ( **customer** ) / Сustomer representativeDevelopment Team |  **_Feature_** Process Description (To Be)CAFDAS/Service architecture (Detailed architecture)StoryDistributive | UAT protocolImplementation OrderCommissioning Order (Optional)Decommissioning Order (Optional)DistributiveA set of scripts and/or configuration files | UAT acceptanceFAT acceptance | Product owner (customer) / Сustomer representativeTesterTeam LeadersCybersecurity ExpertInfrastructure EngineerSupport Engineer | 
| 7 | Implementation/replication | In case of successfully passed UAT, an implementation order is drawn up and agreed upon and the necessary technological changes are initiated. According to results of implementation, results of implementation are recorded | Development Team | Implementation OrderCommissioning Order (Optional)Decommissioning Order (Optional)DistributiveA set of scripts and/or configuration filesUAT protocol | Implementation OrderImplementation Report |  |  | 
| 8 | Operation, support and monitoring |  | OperationsSupport Team | Tested distributive installed on productive environment | Monitoring metrics (optional) |  | Support Engineer | 


## Distribution of responsibility by process steps (RACI matrix)


|  **Abbreviation**  |  **Description**  | 
|  **R**  | Responsible (Executor) - the work executor | 
|  **A**  | Accountable (Responsible) - responsible for work execution and its results | 
|  **C**  | Consult before doing () - expertise that needs to be involved before performing the work | 
|  **I**  | Informed after doing () - participants who need to be notified about results of the work | 





|  **Process step / Role**  |  **Process Owner**  |  **Product owner (customer) / Сustomer representative**  |  **Leader/Head of the Functional Domain (FD)**  |  **Business Analyst**  |  **System Analyst**  |  **Architect**  |  **Designer**  |  **Developer**  |  **Tester**  |  **DevOps Engineer**  |  **Cybersecurity Expert**  |  **Infrastructure Engineer**  |  **Release Manager**  |  **Delivery Manager**  |  **Support Engineer**  | 
|  **_High-level planning_**  |  **I**  |  **R, A**  |  **R, A**  |  **C**  |  **C**  |  **C**  |  |  |  |  |  **C**  |  **C**  |  |  **C**  |  | 
|  **_Analysis_**  |  **I**  |  **C**  |  **C**  |  **R**  |  **C**  |  **C**  |  |  |  |  |  **C**  |  **C**  |  |  **I**  |  | 
|  **_Designing_**  |  **I**  |  **I**  |  **A**  |  **C**  |  **R**  |  **R**  |  |  |  |  |  **C**  |  **C**  |  |  **I**  |  | 
|  **_Decomposition and preparation for implementation_**  |  **I**  |  **C**  |  **R, A**  |  **C**  |  **C**  |  |  |  |  |  |  |  |  **A**  |  **R, A**  |  **I**  | 
|  **_Story implementation_**  |  **I**  |  **I**  |  **R, A**  |  **C**  |  **C**  |  **C**  |  **R**  |  **R**  |  **R**  |  **R**  |  |  **A**  |  **A**  |  **A**  |  | 
|  **_Testing_**  |  **I**  |  **A**  |  **A**  |  |  |  |  |  |  **R**  |  **R**  |  **A**  |  **A**  |  **A**  |  **A**  |  | 
|  **_Implementation/replication_**  |  **I**  |  **I**  |  **C, I**  |  |  |  |  |  |  |  **R**  |  |  **A**  |  **A**  |  **A**  |  **C**  | 
|  **_Operation, support and monitoring_**  |  **I**  |  **C, I**  |  |  |  |  |  |  |  |  |  |  |  |  **C**  |  **R**  | 


1. 
## Process "Story Implementation"

## 2.1.  Process diagram
![](images/storage/SDLC-Story.PNG)
## 2.2.  Tabular description of process diagram


|  **№**  |  **Step's name**  |  **Step description**  |  **Executor**  |  **Input**  |  **Output**  |  **Quality gate**  |  **Responsible for Quality Gate**  | 
| 1 | Planning |  | Leader/Head of the Functional Domain (FD) | Team's backlog (AS/Service/FD) | Sprint |  |  | 
| 2 | Analysis |  | System Analyst |  **_Feature_** Process Description (To Be)CAFDAS/Service architecture (Detailed architecture)StoryDistributive | 
    1. Functional specification document 
    1. Monitoring metrics are defined for automatically feature health checks 

     | FSD approved | Developer | 
| 3 | Designing |  | TesterSystem Analyst | Business monitoring metrics | Test planTest cases | <ul><li>Test plan exists</li><li>Test cases exists</li></ul> | Tester | 
| 4 | Development |  | Developer | StoryFunctional specification document | Source code is in GitAutotests\* | <ul><li>Versioning control</li><li>SonarCube scaning (optional)</li></ul> | DeveloperDevops Engineer | 
| 5 | Testing |  | Tester | DistributiveA set of scripts and/or configuration filesTest planTest cases | Testing reports ST, IFT, LT (optional) | Testing reports ST, IFT, LT (optional) created and filled | Tester | 






## Distribution of responsibility by process steps (RACI matrix)


|  **Abbreviation**  |  **Description**  | 
|  **R**  | Responsible (Executor) - the work executor | 
|  **A**  | Accountable (Responsible) - responsible for work execution and its results | 
|  **C**  | Consult before doing () - expertise that needs to be involved before performing the work | 
|  **I**  | Informed after doing () - participants who need to be notified about results of the work | 





|  **Process step / Role**  |  **Process Owner**  |  **Product owner (customer) / Сustomer representative**  |  **Leader/Head of the Functional Domain (FD)**  |  **Business Analyst**  |  **System Analyst**  |  **Architect**  |  **Designer**  |  **Developer**  |  **Tester**  |  **DevOps Engineer**  |  **Cybersecurity Expert**  |  **Infrastructure Engineer**  |  **Release Manager**  |  **Delivery Manager**  | 
|  **_Planning_**  |  **C, I**  |  **I**  |  **A**  |  |  |  |  |  |  **C**  |  **C**  |  |  |  **C**  |  **R, A**  | 
|  **_Analysis_**  |  **C, I**  |  **I**  |  **C**  |  **C**  |  **R**  |  **C**  |  **C**  |  **C**  |  **C**  |  **C**  |  **C**  |  **C**  |  **C**  |  **A**  | 
|  **_Designing_**  |  **C, I**  |  **I**  |  |  **C**  |  **R**  |  **R**  |  **C**  |  **C**  |  **R**  |  |  **C**  |  **C**  |  |  **A**  | 
|  **_Development_**  |  **C, I**  |  **I**  |  **C**  |  |  |  |  **R**  |  **R**  |  |  **R**  |  |  |  **C**  |  **A**  | 
|  **_Testing_**  |  **C, I**  |  **I**  |  **C**  |  |  |  |  |  |  **R**  |  **R**  |  **C**  |  **C**  |  **C**  |  **A**  | 

 **Annexes** 
## Artifacts used in the SDLC process


| № | Artifact's name | Responsible | Description | Template | 
|  --- |  --- |  --- |  --- |  --- | 
|  **Artifacts that are created once and changed as needed (Describe the current state of the product/solution)**  | 
| 1 | Product vision | Product owner /  **Customer**  | Answers questions:  **what?**    **for whom?**  and  **why?**  we doConsists of:<ul><li>description of the product idea</li><li>description of the values that the product brings</li><li>description of the target audience of the product</li><li>description of strengths and weaknesses, opportunities and threats</li></ul> | [[Product vision|Product-vision]] | 
| 2 | Backlog | Product owner /  **Customer**  | A prioritized list of all known features or outstanding work necessary to bring the product to life. This may include customer/ user needs, technological, functional and non-functional requirements | Report/ Dashboard in JIRA | 
| 3 | CAFD | Architect |  | [Presentation to ArchCom](http://wiki/display/ARCHCOM/Presentation+to+ArchCom) | 
| 4 | AS/Service architecture (Detailed architecture) | Architect/ System Analyst |  | TBD | 
| 5 | Process description | Business Analyst |  | TBD | 
|  **Artifacts "Change " are created in each iteration/sprint (Describe changes in the product/solution)**  | 
| 1 | Feature  | Product owner /  **Customer**  |  | [[Feature|Feature]] | 
| 2 | CR / SR | Product owner /  **Customer**  |  | [[Change Request / Small Request|Change-Request---Small-Request]] | 
|  **Artifacts supplied in each release (Form a release)**  | 
| 1 | Distributive | Developer/ DevOps Engineer | Depends on product team (ZIP, set of scripts and/or configuration files and etc.) |  | 
| 2 | Testing reports ST, IFT, LT | Tester | Link to test run result in Adaptavist Test Management for JIRA and Allure Report[[Software Testing Procedure|Software-Testing-Procedure]] |  | 
| 3 | Test Cases | Tester | [[Software Testing Procedure|Software-Testing-Procedure]] | 250

 | 
| 4 | Test Plan | Tester | [[Software Testing Procedure|Software-Testing-Procedure]] | 250

 | 
| 5 | UAT protocol | Release Manager | [[Software Testing Procedure|Software-Testing-Procedure]] | 250

 | 
| 6 | Implementation Order | Release Manager |  | Status in JIRA | 
| 7 | Commissioning Order (Optional) | Release Manager |  | Status in JIRA | 
| 8 | Decommissioning Order (Optional) | Release Manager |  | Status in JIRA | 
| 9 | Implementation Report | Release Manager |  | Status in JIRA | 


## Matching process objects and JIRA objects

```

```


| 1 | Project | Project | 
| 2 | Feature | Epic | 
| 3 | CR / SR | Story (SR) | 
| 4 | Technological debt | Task | 
| 5 | Bug | Bug | 


## The scheme of interaction of process objects in JIRA
![](images/storage/SDLC-JIRA.png)

Files and Documents

| File Description | Link | 
|  --- |  --- | 
| SDLC Document | 250

 | 
|  |  | 





*****

[[category.storage-team]] 
[[category.confluence]] 
