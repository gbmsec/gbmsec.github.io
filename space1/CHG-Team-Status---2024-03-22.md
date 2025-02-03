





| CHG

 | 
| Alexey

 | 
| 

 | 
| Calypso:<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - делаем доработки по MiFID Transaction Report. Тестирование загрузки биржевых сделок из экспортера QUIK. Тестируем доработки по FATCA / CRS отчетам. Обсуждаем требования по реализации агентской схемы и CFD. Работаем над массовой загрузкой CDS из файла.</li><li>BCSGL - делаем мелкие доработки по TSL. </li><li>BCSUK - подготовили данные по количеству ISIN за год для предоставления в CUSIP. Работаем над исправлением багов, которые нам пришли от Баско.</li></ul>IBQ: Продолжаем делать аналитику и разработку по проекту EMIR Refit. Провели тестирование по двум критичным SR по загрузке неторговый поручений и DVP / RVP сделокKondor
1.  **Ресурсная проблема отсутствия разработчика создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Вывели интеграцию с ТОМС на Кипре.
1. Систематика подготовила CW и установила в нашей тестовой системе. Можно разрабатывать нашу интеграцию полностью.
1. Запустили подготовительный процесс согласования BRD на Атриум.

ESB<ul><li>ESB internal tasks and bugs</li><li>EP. Upgrade Artemis to UK state</li><li>Sending mail via EWS</li><li>EP. Upgrade ESB version</li></ul>Riskroom:<ul><li>started to analyze tasks related to decommission of Qort</li><li>one more SR for EMIR-REFIT went live (CMA room enhancements for CDS portfolio calc)</li><li>started to analyze what is also unused at UK to switch off</li></ul>FX:<ul><li>Still having of time requests to database from ntpro2db - timeout enlarged, implemented to prod, to monitor - missed to proceed on that</li><li>Banded tariffication - installed to prod, working on more issues found</li><li>Unusual client activity alarm is at prod, more task to show it at UI</li><li>DynRep: started to develop, no test data for corpm switched to another part</li><li>News portal: minor changes, also to sort out some users do have some role (still no feedback on that)</li></ul>OneTick, SFTR:<ul><li>OneTick: started implementation for markit</li><li>Murex project: some minor activities, waiting for analysis</li><li>to plan new SR (qustionnarie) - analysis</li></ul>EMIR/REFIT:<ul><li>Oleg/Stas are working on the tasks</li><li>Igor finished working on UTI generation task at IBQ, testing</li><li>Igor is finishing Anna DSB data load</li><li>Stas is finishing FIRDS loader to EDW service</li></ul>RegReporting<ul><li>To be architecture draft is done - to enhance further - no resources this week</li></ul>EDW<ul><li>Emir-Refit margin report functionality is testing - bugfixing</li><li>Test activities support required to fix Qort load</li><li>new SR (SFTR qustionnarie) development is done, testing</li><li>to stop NSD services at UK (not done)</li></ul> | 
| top 3-5 points | 
| 1) ОХД - есть проблема с ресурсами. Не можем делать в параллель 3 активности, а только одну. Из набора Декомиссия, Марекс, cfd надо выбирать чем заниматься2) Есть проблема с подготовкой данный для ispiral. Давай обсудим, надо как то ускорять3) Ольга Ш - декрет с июля. Это меняет все планы по ставкам и срокам4) Есть проблема с Графаной, которая может сильно испортить взаимодействия в коллективе.5) Нужно решение по рег репортингу на Кипр. Сейчас тратим время6) IBQ DR сервер. надо дать команду его доделать (ресурс Олега Е) **Services escalation from Kostya** edw tasks related to existing functionality are very slow to resolve, there risks of delay for testing emir-refitreqs for OT - markit - only today news arrived for 3 files instead of 1, huge risk not to meet net week to go live | 
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
| Calypso:<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - делаем доработки по MiFID Transaction Report. Тестирование загрузки биржевых сделок из экспортера QUIK. Тестируем доработки по FATCA / CRS отчетам. Обсуждаем требования по реализации агентской схемы и CFD. Работаем над массовой загрузкой CDS из файла.</li><li>BCSGL - делаем мелкие доработки по TSL. </li><li>BCSUK - подготовили данные по количеству ISIN за год для предоставления в CUSIP. Работаем над исправлением багов, которые нам пришли от Баско.</li></ul>IBQ: Продолжаем делать аналитику и разработку по проекту EMIR Refit. Провели тестирование по двум критичным SR по загрузке неторговый поручений и DVP / RVP сделокKondor
1.  **Ресурсная проблема отсутствия разработчика создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Вывели интеграцию с ТОМС на Кипре.
1. Систематика подготовила CW и установила в нашей тестовой системе. Можно разрабатывать нашу интеграцию полностью.
1. Запустили подготовительный процесс согласования BRD на Атриум.

ESB<ul><li>ESB internal tasks and bugs</li><li>EP. Upgrade Artemis to UK state</li><li>Sending mail via EWS</li><li>EP. Upgrade ESB version</li></ul>Riskroom:<ul><li>started to analyze tasks related to decommission of Qort</li><li>one more SR for EMIR-REFIT went live (CMA room enhancements for CDS portfolio calc)</li><li>started to analyze what is also unused at UK to switch off</li></ul>FX:<ul><li>Still having of time requests to database from ntpro2db - timeout enlarged, implemented to prod, to monitor - missed to proceed on that</li><li>Banded tariffication - installed to prod, working on more issues found</li><li>Unusual client activity alarm is at prod, more task to show it at UI</li><li>DynRep: started to develop, no test data for corpm switched to another part</li><li>News portal: minor changes, also to sort out some users do have some role (still no feedback on that)</li></ul>OneTick, SFTR:<ul><li>OneTick: started implementation for markit</li><li>Murex project: some minor activities, waiting for analysis</li><li>to plan new SR (qustionnarie) - analysis</li></ul>EMIR/REFIT:<ul><li>Oleg/Stas are working on the tasks</li><li>Igor finished working on UTI generation task at IBQ, testing</li><li>Igor is finishing Anna DSB data load</li><li>Stas is finishing FIRDS loader to EDW service</li></ul>RegReporting<ul><li>To be architecture draft is done - to enhance further - no resources this week</li></ul>EDW<ul><li>Emir-Refit margin report functionality is testing - bugfixing</li><li>Test activities support required to fix Qort load</li><li>new SR (SFTR qustionnarie) development is done, testing</li><li>to stop NSD services at UK (not done)</li></ul> | 
| top 3-5 points | 
| 1) ОХД - есть проблема с ресурсами. Не можем делать в параллель 3 активности, а только одну. Из набора Декомиссия, Марекс, cfd надо выбирать чем заниматься2) Есть проблема с подготовкой данный для ispiral. Давай обсудим, надо как то ускорять3) Ольга Ш - декрет с июля. Это меняет все планы по ставкам и срокам4) Есть проблема с Графаной, которая может сильно испортить взаимодействия в коллективе.5) Нужно решение по рег репортингу на Кипр. Сейчас тратим время6) IBQ DR сервер. надо дать команду его доделать (ресурс Олега Е) **Services escalation from Kostya** edw tasks related to existing functionality are very slow to resolve, there risks of delay for testing emir-refitreqs for OT - markit - only today news arrived for 3 files instead of 1, huge risk not to meet net week to go live | 







*****

[[category.storage-team]] 
[[category.confluence]] 
