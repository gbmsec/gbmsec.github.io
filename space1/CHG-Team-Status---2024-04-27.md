





| CHG

 | 
| Alexey

 | 
| 

 | 
| Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - выводим первую версию по FX Netting Confirmation. В процессе разработки по MiFID Transactions. Делаем багфиксинг по ликвидити репорту. Отдали в тестирование Currency Cintrol Report. Загрузили сделки CDS с текущего кипра в Calypso PRODCY.</li><li>BCSGL - получили новые требования на доработку TSL. С релизом выкатываем настройки по загрузке биржевых сделок с экспортера QUIK.</li><li>BCSUK - С релизом выходят доработки по MiFID Post Trade Reporting и задача по переключения загрузки CA вместо Маркита на Евроклир</li></ul>

<ul><li>IBQ:</li></ul><ul><li>Проводим UAT по проекту EMIR Refit + багфиксинг. </li><li>Вывели новый сервис EMIR Refit на PROD  </li><li>Выводим релиз IBQ 2.0 </li><li>Довыгрузили данные по годовой отчетности Кипра</li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>EP. Upgrade ESB version 3.20.9 → 3.22.1</li><li>BPM. Helper services on ESB</li><li>SF → KHD new flows</li><li>EP. Calypso → Ibank</li></ul>Kondor
1. OpenTRM - прошли безопасность, подготовили и посалали на внутреннее согласование контракт.
1. Распределил контакты для Систематики - к кому обращаться в случае каких вопросов.
1. Отладка || run шлюза - прогружены по возможности сделки FxSpot и Equities, получены вопросы от Систематики - решены на 80%.
1. Скоординированы внутри команды работы над ошибками в отладке || run шлюза.
1. От бизнеса получен окончательный список счетов, которые нужны в Атриуме.

Riskroom:<ul><li>SL3 for Repo room due to BBG and Quik prices conflict, solution is in progress along with GBX rate</li><li>continue to analyze and implement tasks related to decommission of Qort</li><li>moving Quik autolimits functionality to EP - in progress - wait for Quik to analyze at their side</li><li>ARM RM limits - new enhancements were delivered, waiting for feedback</li></ul>FX:<ul><li>Unusual client activity added to UI: UAT continues</li><li>Some minor fixes for adding new pairs, etc.</li><li>DynRep: no development until single view is ready at IBSO side</li></ul>OneTick, SFTR, Regreporting:<ul><li>SFTR change for SFTR questionnarie is deployed to prod</li><li>OneTick: implementation for marex - deployed to prod</li><li>Data supermarket UI service hotfixed after new role added for regreporting</li><li>SFTR hotfixed after new data started to arrive on new SF Questionnarie</li><li>Discussions on reporting service approach, Draft demo was discussed with AVyugovskiy, not much progress this week</li></ul>EMIR/REFIT: Many release and support problems were solvedEDW<ul><li>Prepare for Emir-Refit release:<ul><li>EDW - changes went live</li><li>AnnaDSB loader service - went live</li><li>Firds-EDW loader service - went live</li></ul></li><li>new SR (SFTR qustionnarie) development is done, deployed to prod</li><li>to stop NSD services at UK (not done)</li></ul>Others - CBONDs rating service: investigating request from group risks on missing data | 
| top 3-5 points | 
|  | 
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
| Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - выводим первую версию по FX Netting Confirmation. В процессе разработки по MiFID Transactions. Делаем багфиксинг по ликвидити репорту. Отдали в тестирование Currency Cintrol Report. Загрузили сделки CDS с текущего кипра в Calypso PRODCY.</li><li>BCSGL - получили новые требования на доработку TSL. С релизом выкатываем настройки по загрузке биржевых сделок с экспортера QUIK.</li><li>BCSUK - С релизом выходят доработки по MiFID Post Trade Reporting и задача по переключения загрузки CA вместо Маркита на Евроклир</li></ul>

<ul><li>IBQ:</li></ul><ul><li>Проводим UAT по проекту EMIR Refit + багфиксинг. </li><li>Вывели новый сервис EMIR Refit на PROD  </li><li>Выводим релиз IBQ 2.0 </li><li>Довыгрузили данные по годовой отчетности Кипра</li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>EP. Upgrade ESB version 3.20.9 → 3.22.1</li><li>BPM. Helper services on ESB</li><li>SF → KHD new flows</li><li>EP. Calypso → Ibank</li></ul>Kondor
1. OpenTRM - прошли безопасность, подготовили и посалали на внутреннее согласование контракт.
1. Распределил контакты для Систематики - к кому обращаться в случае каких вопросов.
1. Отладка || run шлюза - прогружены по возможности сделки FxSpot и Equities, получены вопросы от Систематики - решены на 80%.
1. Скоординированы внутри команды работы над ошибками в отладке || run шлюза.
1. От бизнеса получен окончательный список счетов, которые нужны в Атриуме.

Riskroom:<ul><li>SL3 for Repo room due to BBG and Quik prices conflict, solution is in progress along with GBX rate</li><li>continue to analyze and implement tasks related to decommission of Qort</li><li>moving Quik autolimits functionality to EP - in progress - wait for Quik to analyze at their side</li><li>ARM RM limits - new enhancements were delivered, waiting for feedback</li></ul>FX:<ul><li>Unusual client activity added to UI: UAT continues</li><li>Some minor fixes for adding new pairs, etc.</li><li>DynRep: no development until single view is ready at IBSO side</li></ul>OneTick, SFTR, Regreporting:<ul><li>SFTR change for SFTR questionnarie is deployed to prod</li><li>OneTick: implementation for marex - deployed to prod</li><li>Data supermarket UI service hotfixed after new role added for regreporting</li><li>SFTR hotfixed after new data started to arrive on new SF Questionnarie</li><li>Discussions on reporting service approach, Draft demo was discussed with AVyugovskiy, not much progress this week</li></ul>EMIR/REFIT: Many release and support problems were solvedEDW<ul><li>Prepare for Emir-Refit release:<ul><li>EDW - changes went live</li><li>AnnaDSB loader service - went live</li><li>Firds-EDW loader service - went live</li></ul></li><li>new SR (SFTR qustionnarie) development is done, deployed to prod</li><li>to stop NSD services at UK (not done)</li></ul>Others - CBONDs rating service: investigating request from group risks on missing data | 
| top 3-5 points | 
|  | 







*****

[[category.storage-team]] 
[[category.confluence]] 
