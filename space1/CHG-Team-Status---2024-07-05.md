





| CHG

 | 
| Alexey

 | 
| 

 | 
| Riskroom:

<ul><li>continue to analyze and implement tasks related to decommission of Qort (deal from Calypso OK, need user setup of accounts to produce limit files), continued to implement parallel run for Eligible2022 with Calypso, also limits generation. There was some progress to map Qort vs Calypso data, some questions asked, need clarification</li><li>implemented change for Eligible2022 CY report so it reduces requests to BBG for static date, deployed to prod, required HF next day, done</li><li>moving Quik autolimits functionality to EP - in progress - wait for Quik to get licence - on hold at RR side</li><li>ARM RM limits - need to analyze Credit limit, awaiting details on Calypso data to use - there was a meeting with Nikita Bobrov. Looks like we need internal actual settled pos for agent type of accounts, Risks are analyzing </li></ul>FX:

<ul><li>Implemented new functionality for alerting on rejected deals - deployed</li><li>DynRep: single view is ready at IBSO side, waiting for analysis to start dev</li><li>Todo: add auth to News service API, as it is going to be reused by desk itself</li><li>HF had to be done as database job fails, had to refactor a stored procedure Trades_juridical_upd_check</li><li>New and probably urgent task to change TOM to TOD, need analysis to complete</li></ul>OneTick, SFTR, Regreporting:

<ul><li>Reporting services: discussed approach to get Calypso data: still in progress on Calypso side</li><li>SFTR: analysis is ready for 1 task, taken in dev by Oleg</li><li>Continued to investigate high priority issue with FCA recon</li></ul>EDW

<ul><li>Started working on a data loader service not to depend on PL/SQL (refactoring of KHD prices load routine - as a first target)</li><li>to stop NSD services at UK (not done)</li><li>some SL3 tasks todo</li><li>deploy at UK fixed</li><li>monitoring on UK: clarified nature of issues, decided to move monitoring run</li></ul>NTOe v2

<ul><li>Moving forward with backend for it ([Back-end (Draft)](http://wiki/pages/viewpage.action?pageId=1238761484))</li><li>Draft UI is on its way</li><li>Started to project role model, did some progress</li><li>Need analysis on attributes</li></ul>Others

<ul><li>CBONDs rating service: need to consider moving to KHD to get data, as they are implementing such CBONDs integration on their side (todo)</li><li>Product governance service: participate in planning and discussions</li></ul>

CRM

1) Product Governance

<ul><li>Requirements clarified</li><li>Web form for collecting all data in development</li><li>New product governance fields are added to Salesforce</li></ul>2) BPM Soft - exploration, tryout of developing MVP for RU process (best efforts)

3) EMIR SFTR - wiki documentation for delivered fuctionality

4) Project K

<ul><li>Developemetn of web forms to set up Individual/Institutional clients to IB for new CY business</li><li>Waiting for client data exports from EVA & BOMR</li></ul>5) Full scope of integration of Contacts from SF to Calypso - discussions with BO colleagues.



Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li></ul></li></ul><ul><li>BCSCY - доделали задачи в релиз по агентскому РЕПО, формированию UTI и проставлению места хранения на комиссии в NTO. Закончили SHS выгрузку данных для Reporting Service. Сделали доработку в Request Reply процессе по запросу данных из Калипсо.</li><li>BCSGL - в релиз выходят новая сверка с БКС банком</li><li>BCSUK - настроили редемпшн по бондам для финансов. Расчет EIR передали в разработку. После релиза сделаем очистку статики в UK по данным BCSCY, BCSUS и BCSGL.</li></ul>IBQ:

<ul><li>Работа над задачами. Взяли в работу критичные SR по SFTR. Делаем багфиксинг по найденным проблемам прода.</li><li>Согласовали процесс Request Reply между Reporting Service и Calypso по получению данных из Calypso.</li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>UK. Upgrade ESB version 3.22.1 → 4.4.2</li><li>EP. SF - Calypso changes</li><li>Remove ESB UK - DB nonUK links</li></ul>Kondor
1. Отладка || run шлюза движется к финальной стадии. В последней итерации тестирования загрузки первоначального snap-shot были только 2 ошибки.
1. Проведена встреча с проектной командой PRJ-314 (декомиссия Корта). Проработаны совместные шаги и способы взаимодействия.
1. Product governance - на стадии открытия проекта.
1. Проведена встреча с ОХД и Бухгалтерией для уточнения их использования данных из К+ с целью оптимального перенесения его в Атриум
1. Новый разработчик полностью ведет задачу по разработке сверки для || run шлюза (под контролем и тестировании задачи аналитиком, по процессу).

 | 
| top 3-5 points | 
| Согласовали с ДЗ что разделяем Жиру после создания почты на ЮК, разделение Жиры перенеслиКалипсо ЮК отключили от Группы.Вики разделим на этих выходныхСогласовали открытие проекта Product governance.На этих выходных технически запускаем Атриум (||-run)большие направления работы1) Передача дел по АМЛ. Тут надо попробовать перенести сервис на нашу инфру. Для этого надо согласовать перенос данных (БД). Сейчас заблокированы на ДИБ.2) УКФ на Кипре - пока не было звонков. Попросил начать созвоны. На след неделе будем инфру обсуждать.3) Варианты решение и ускорения по ОХД в части Корта-Калипсо. Ждем оценок привлечения вендора.HRближайшие выходы: Сергиенко (12-07), Василий Старцев (15-07)прислали новых резюме на аналитика НТОЕ, отправил акцепт на 3х кандидатов, собесов на этой неделе не было. | 
|  --- | 
|  --- | 
|  --- | 
|  --- | 
|  --- | 
|  --- | 
| CHG

 | 
| Alexey

 | 
| 

 | 
| Riskroom:

<ul><li>continue to analyze and implement tasks related to decommission of Qort (deal from Calypso OK, need user setup of accounts to produce limit files), continued to implement parallel run for Eligible2022 with Calypso, also limits generation. There was some progress to map Qort vs Calypso data, some questions asked, need clarification</li><li>implemented change for Eligible2022 CY report so it reduces requests to BBG for static date, deployed to prod, required HF next day, done</li><li>moving Quik autolimits functionality to EP - in progress - wait for Quik to get licence - on hold at RR side</li><li>ARM RM limits - need to analyze Credit limit, awaiting details on Calypso data to use - there was a meeting with Nikita Bobrov. Looks like we need internal actual settled pos for agent type of accounts, Risks are analyzing </li></ul>FX:

<ul><li>Implemented new functionality for alerting on rejected deals - deployed</li><li>DynRep: single view is ready at IBSO side, waiting for analysis to start dev</li><li>Todo: add auth to News service API, as it is going to be reused by desk itself</li><li>HF had to be done as database job fails, had to refactor a stored procedure Trades_juridical_upd_check</li><li>New and probably urgent task to change TOM to TOD, need analysis to complete</li></ul>OneTick, SFTR, Regreporting:

<ul><li>Reporting services: discussed approach to get Calypso data: still in progress on Calypso side</li><li>SFTR: analysis is ready for 1 task, taken in dev by Oleg</li><li>Continued to investigate high priority issue with FCA recon</li></ul>EDW

<ul><li>Started working on a data loader service not to depend on PL/SQL (refactoring of KHD prices load routine - as a first target)</li><li>to stop NSD services at UK (not done)</li><li>some SL3 tasks todo</li><li>deploy at UK fixed</li><li>monitoring on UK: clarified nature of issues, decided to move monitoring run</li></ul>NTOe v2

<ul><li>Moving forward with backend for it ([Back-end (Draft)](http://wiki/pages/viewpage.action?pageId=1238761484))</li><li>Draft UI is on its way</li><li>Started to project role model, did some progress</li><li>Need analysis on attributes</li></ul>Others

<ul><li>CBONDs rating service: need to consider moving to KHD to get data, as they are implementing such CBONDs integration on their side (todo)</li><li>Product governance service: participate in planning and discussions</li></ul>

CRM

1) Product Governance

<ul><li>Requirements clarified</li><li>Web form for collecting all data in development</li><li>New product governance fields are added to Salesforce</li></ul>2) BPM Soft - exploration, tryout of developing MVP for RU process (best efforts)

3) EMIR SFTR - wiki documentation for delivered fuctionality

4) Project K

<ul><li>Developemetn of web forms to set up Individual/Institutional clients to IB for new CY business</li><li>Waiting for client data exports from EVA & BOMR</li></ul>5) Full scope of integration of Contacts from SF to Calypso - discussions with BO colleagues.



Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li></ul></li></ul><ul><li>BCSCY - доделали задачи в релиз по агентскому РЕПО, формированию UTI и проставлению места хранения на комиссии в NTO. Закончили SHS выгрузку данных для Reporting Service. Сделали доработку в Request Reply процессе по запросу данных из Калипсо.</li><li>BCSGL - в релиз выходят новая сверка с БКС банком</li><li>BCSUK - настроили редемпшн по бондам для финансов. Расчет EIR передали в разработку. После релиза сделаем очистку статики в UK по данным BCSCY, BCSUS и BCSGL.</li></ul>IBQ:

<ul><li>Работа над задачами. Взяли в работу критичные SR по SFTR. Делаем багфиксинг по найденным проблемам прода.</li><li>Согласовали процесс Request Reply между Reporting Service и Calypso по получению данных из Calypso.</li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>UK. Upgrade ESB version 3.22.1 → 4.4.2</li><li>EP. SF - Calypso changes</li><li>Remove ESB UK - DB nonUK links</li></ul>Kondor
1. Отладка || run шлюза движется к финальной стадии. В последней итерации тестирования загрузки первоначального snap-shot были только 2 ошибки.
1. Проведена встреча с проектной командой PRJ-314 (декомиссия Корта). Проработаны совместные шаги и способы взаимодействия.
1. Product governance - на стадии открытия проекта.
1. Проведена встреча с ОХД и Бухгалтерией для уточнения их использования данных из К+ с целью оптимального перенесения его в Атриум
1. Новый разработчик полностью ведет задачу по разработке сверки для || run шлюза (под контролем и тестировании задачи аналитиком, по процессу).

 | 
| top 3-5 points | 
| Согласовали с ДЗ что разделяем Жиру после создания почты на ЮК, разделение Жиры перенеслиКалипсо ЮК отключили от Группы.Вики разделим на этих выходныхСогласовали открытие проекта Product governance.На этих выходных технически запускаем Атриум (||-run)большие направления работы1) Передача дел по АМЛ. Тут надо попробовать перенести сервис на нашу инфру. Для этого надо согласовать перенос данных (БД). Сейчас заблокированы на ДИБ.2) УКФ на Кипре - пока не было звонков. Попросил начать созвоны. На след неделе будем инфру обсуждать.3) Варианты решение и ускорения по ОХД в части Корта-Калипсо. Ждем оценок привлечения вендора.HRближайшие выходы: Сергиенко (12-07), Василий Старцев (15-07)прислали новых резюме на аналитика НТОЕ, отправил акцепт на 3х кандидатов, собесов на этой неделе не было. | 







*****

[[category.storage-team]] 
[[category.confluence]] 
