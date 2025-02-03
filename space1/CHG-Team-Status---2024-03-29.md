





| CHG

 | 
| Alexey 

 | 
| 

 | 
| Riskroom:

<ul><li>Repo room missing GBX price investigation</li><li>continue to analyze tasks related to decommission of Qort</li><li>continue to analyze what is also unused at UK to switch off</li><li>new task "Limits to MM" was initially discussed, waiting for SR and reqs - Это нежданьчик и незапланированная задача по market making на AIX</li></ul>FX:

<ul><li>Banded tariffication - installed to prod, working on more issues found - patch release applied to prod</li><li>Unusual client activity alarm is at prod, more task to show it at UI - UAT deployed</li><li>DynRep: stopping development until stable prod-like env for testing</li><li>Prepare for agile committee</li></ul>OneTick, SFTR:

<ul><li>OneTick: implementation for markit - UAT, new reqs arrives</li><li>Murex project: some minor activities, waiting for analysis</li><li>to plan new SR (qustionnarie) - analysis - still question if any changes needed</li></ul>EMIR/REFIT:

<ul><li>Oleg/Stas are working on the tasks</li><li>Igor finished working on UTI generation task at IBQ, testing</li><li>Igor is finishing Anna DSB data load</li><li>Stas is finishing FIRDS loader to EDW service</li></ul>RegReporting

<ul><li>To be architecture draft is done - to enhance further - no resources this week</li></ul>EDW

<ul><li>Emir-Refit margin report functionality is testing - bugfixing</li><li>Test activities support required to fix Qort load</li><li>new SR (SFTR qustionnarie) development is done, testing</li><li>to stop NSD services at UK (not done)</li></ul>

ESB

<ul><li>ESB internal tasks and bugs</li><li>EP. Upgrade ESB version + unit tests setup</li><li>UK. Upgrade ESB version + unit tests setup</li><li>BPM. Helper services on ESB</li></ul>

Kondor


1. Идет on-boarding разработчика. Прям по профилю найти не вышло, нашли с квалификацией SQL и XML (немного VBS).
1. On-bording OpenTRM в процессе. Мое мнение - останавливать не надо, работы много, особенно с учетом нижеследующих пунктов.
1. От бизнеса приходят "срочные" задачи (что вне проекта Атриум): загрузка и учет дат офферт облигаций, Product Governance. Ресурсов на них нет.  **Непонятно, как и с кем согласовывать снятие ресурсов с проекта перехода на Атриум на срочные задачи других направлений - что повлечет за собой сдвиг сроков проекта Атриум.** 
1. Проведена межпроектная встреча по интеграции Атриум - Калипсо (Кипр ИБ). Обсуждены сроки и общие подходы. На апрель запланировано тестирование интеграции Атриум2Калипсо.
1. Начали разработку интеграции полностью - с полями CW.



CRM

 **EMIR REFIT** 

<ul><li>FA → SF integrational developement</li><li>Process tests</li></ul> **Service Cloud - ** Processing order with ITVM

 **SF CY data clearance ** 

<ul><li>Clearing unnecessary data</li><li>Analysing tactical and strategical options</li><li>Clearing/Modifying unnecessary processes</li><li>establishing new basic process and data</li><li>Troubleshooting with KHD</li><li>testing</li></ul> **Project K - ** Data migration discussions and requests



Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - сетап продукта CDS завершен. Тестируем FX Netting Confo. Тестирование отчетов по MiFID / FATCA / CRS. Тестируем в рамках UAT загрузку биржевых сделок из QUIK экспортера.</li><li>BCSGL - багфиксинг и новые небольшие доработки по TSL</li><li>BCSUK - отправили отчет в рамках аудита по CUSIP. Сделали исправление по MiFID Post trade reporting.</li></ul>

IBQ:

<ul><li>Продолжаем делать аналитику и разработку по проекту EMIR Refit.</li><li>По результатам встречи по SR взяли новые три REQ задачи в работу по IBQ</li></ul>

 | 
| top 3-5 points | 
| 1) ОХД 1.1) в работе - справочники по субъектам и субсчетам. Сделки еще не начинали. В целом можно оценить, что от общего объема работы в работе или сделано не более 10%. Достаточно слабо. 1.2) Марекс. Обратная связь такова, что потратили очень много времени на тестирование. Работают с 29 февраля. Было много переделок, перетестирований, перезаведения сдлок. Тестовые примеры были с ошибками. ресурсов потрачено очень много на ОХД и на получателях на этой активности. 1.3) нет новостей по разработчику Николай на ОХД. вроде пока так же собирается увольняться.2) По мониторигу. Хотели улучшить и сделать мониторинг Графана-ЕДВ на нон-ЮК. Макс сказал, что не сможет, т.к. плагин к Оракту платный. Плохл. Что делать будем ? Если не покупать, то считай нет мониторинга по ЕДВ на нон-ЮК.3) Договор с OpenTRM. Еще не запускали в согласование в ШП.4) Договор с ВДКом на апрель-июнь. идет согласование, не закончено еще.  5) Оплата ВДКом февраль. Заведут в оплату только сегодня 29-03-24. 6) по принятию рисков работы без договра ты не ответил7) ЮК. Данные по аудиту на калипсо на диске Р. Сейчас больше ничего не готовим, ждем прояснений от аудиторов.8) Проблема с процессингом платежей, договоров. Мало ресурса на этом направлении | 
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

<ul><li>Repo room missing GBX price investigation</li><li>continue to analyze tasks related to decommission of Qort</li><li>continue to analyze what is also unused at UK to switch off</li><li>new task "Limits to MM" was initially discussed, waiting for SR and reqs - Это нежданьчик и незапланированная задача по market making на AIX</li></ul>FX:

<ul><li>Banded tariffication - installed to prod, working on more issues found - patch release applied to prod</li><li>Unusual client activity alarm is at prod, more task to show it at UI - UAT deployed</li><li>DynRep: stopping development until stable prod-like env for testing</li><li>Prepare for agile committee</li></ul>OneTick, SFTR:

<ul><li>OneTick: implementation for markit - UAT, new reqs arrives</li><li>Murex project: some minor activities, waiting for analysis</li><li>to plan new SR (qustionnarie) - analysis - still question if any changes needed</li></ul>EMIR/REFIT:

<ul><li>Oleg/Stas are working on the tasks</li><li>Igor finished working on UTI generation task at IBQ, testing</li><li>Igor is finishing Anna DSB data load</li><li>Stas is finishing FIRDS loader to EDW service</li></ul>RegReporting

<ul><li>To be architecture draft is done - to enhance further - no resources this week</li></ul>EDW

<ul><li>Emir-Refit margin report functionality is testing - bugfixing</li><li>Test activities support required to fix Qort load</li><li>new SR (SFTR qustionnarie) development is done, testing</li><li>to stop NSD services at UK (not done)</li></ul>

ESB

<ul><li>ESB internal tasks and bugs</li><li>EP. Upgrade ESB version + unit tests setup</li><li>UK. Upgrade ESB version + unit tests setup</li><li>BPM. Helper services on ESB</li></ul>

Kondor


1. Идет on-boarding разработчика. Прям по профилю найти не вышло, нашли с квалификацией SQL и XML (немного VBS).
1. On-bording OpenTRM в процессе. Мое мнение - останавливать не надо, работы много, особенно с учетом нижеследующих пунктов.
1. От бизнеса приходят "срочные" задачи (что вне проекта Атриум): загрузка и учет дат офферт облигаций, Product Governance. Ресурсов на них нет.  **Непонятно, как и с кем согласовывать снятие ресурсов с проекта перехода на Атриум на срочные задачи других направлений - что повлечет за собой сдвиг сроков проекта Атриум.** 
1. Проведена межпроектная встреча по интеграции Атриум - Калипсо (Кипр ИБ). Обсуждены сроки и общие подходы. На апрель запланировано тестирование интеграции Атриум2Калипсо.
1. Начали разработку интеграции полностью - с полями CW.



CRM

 **EMIR REFIT** 

<ul><li>FA → SF integrational developement</li><li>Process tests</li></ul> **Service Cloud - ** Processing order with ITVM

 **SF CY data clearance ** 

<ul><li>Clearing unnecessary data</li><li>Analysing tactical and strategical options</li><li>Clearing/Modifying unnecessary processes</li><li>establishing new basic process and data</li><li>Troubleshooting with KHD</li><li>testing</li></ul> **Project K - ** Data migration discussions and requests



Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - сетап продукта CDS завершен. Тестируем FX Netting Confo. Тестирование отчетов по MiFID / FATCA / CRS. Тестируем в рамках UAT загрузку биржевых сделок из QUIK экспортера.</li><li>BCSGL - багфиксинг и новые небольшие доработки по TSL</li><li>BCSUK - отправили отчет в рамках аудита по CUSIP. Сделали исправление по MiFID Post trade reporting.</li></ul>

IBQ:

<ul><li>Продолжаем делать аналитику и разработку по проекту EMIR Refit.</li><li>По результатам встречи по SR взяли новые три REQ задачи в работу по IBQ</li></ul>

 | 
| top 3-5 points | 
| 1) ОХД 1.1) в работе - справочники по субъектам и субсчетам. Сделки еще не начинали. В целом можно оценить, что от общего объема работы в работе или сделано не более 10%. Достаточно слабо. 1.2) Марекс. Обратная связь такова, что потратили очень много времени на тестирование. Работают с 29 февраля. Было много переделок, перетестирований, перезаведения сдлок. Тестовые примеры были с ошибками. ресурсов потрачено очень много на ОХД и на получателях на этой активности. 1.3) нет новостей по разработчику Николай на ОХД. вроде пока так же собирается увольняться.2) По мониторигу. Хотели улучшить и сделать мониторинг Графана-ЕДВ на нон-ЮК. Макс сказал, что не сможет, т.к. плагин к Оракту платный. Плохл. Что делать будем ? Если не покупать, то считай нет мониторинга по ЕДВ на нон-ЮК.3) Договор с OpenTRM. Еще не запускали в согласование в ШП.4) Договор с ВДКом на апрель-июнь. идет согласование, не закончено еще.  5) Оплата ВДКом февраль. Заведут в оплату только сегодня 29-03-24. 6) по принятию рисков работы без договра ты не ответил7) ЮК. Данные по аудиту на калипсо на диске Р. Сейчас больше ничего не готовим, ждем прояснений от аудиторов.8) Проблема с процессингом платежей, договоров. Мало ресурса на этом направлении | 







*****

[[category.storage-team]] 
[[category.confluence]] 
