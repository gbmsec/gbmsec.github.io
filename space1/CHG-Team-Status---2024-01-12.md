





| CHG

 | 
| Alexey

 | 
| 

 | 
| Calypso:

<ul><li>Из проектов работаем над задачами: Setup BCSCY in Calypso Non UK, CASS</li></ul><ul><li>CASS - исправили проблему по автосетелменту сделок для BCSCY</li><li>BCSCY - сделали сетап ОТС equity option, делали правки по SWIFT инструктированию + неттинг конфо.</li><li>BCSGL - были сделаны донастройки конфигурации в TSL по сделкам, которые есть на PRODCY</li><li>Развернули локально новый инстанс Calypso 17 на NV в UK, чтобы на нем провести регрессионное тестирование текущего функционала. </li></ul>IBQ:

<ul><li>Продолжаем делать аналитику по проекту EMIR Refit. Делаем разработку по формированию файлов EMIR c Trade Report по описанным продуктам. Сделали багфиксинг мелких проблем прода + пара SR-ов к релизу.</li><li>Новый аналитик на аутсорс закончил заниматься задачами на OneTick и переключается на задачу по загрузке данных из Anna DSB для EMIR Refit.</li><li>В праздники сломались диски на сервере, где располагался application QORT ТЧК, сейчас сервер восстановили, занимаемся восстановлением тестового контура QORT.</li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>UK ESB Upgrade: properties and master-lock</li><li>Backlog tasks</li><li>integration with RJOB portal</li></ul>Kondor
1.  **Ресурсная проблема создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Систематика заявила, что они остаются при своем мнении по требованиям к HW, а значит не могут гарантировать заявленной производительности Атриума.
1. В релизе 12.01.24 запланирован вывод задачи по обогащению post-trade репортинга (давно запрошено комплаенсом), а также переключаемся на nonUK почтовый сервер.
1. Получены новые требования по проекту выпуска нот на Казахстане - обработка FX Spot сделок.

 **CRM** 1) Migration of UK CRM service:<ul><li>Migration of metadata ongoing</li><li>Discussing and justifying plan dates for UK PMO</li><li>Request for prolongation of old ogr for 12 days was sent to UK Salesforce - pending answer</li><li>Invoice for new UK org was paid</li></ul>2) MRRA separation on EMIR & SFTR agreement types - separated Agreement types on TEST, provided TEST data to colleagues from EDW3) Full CY clientbase upload & support in CRM - Preparatiopn of full list of required data with format and comments4) Hotifx for UK users rights in old org: making them independant from non-UK sales users approval's on work with client baseRiskroom:<ul><li>SR for FX room delivered to production</li><li>FI related SR is in development and analysis</li></ul>FX:<ul><li>Dev continues for banded tariffication, delployed to UAT, procedural API for bank agreed, testing starting</li><li>Investigate deadlock issue: need to fix WeekendRates service to set transaction level - Snapshot</li><li>EWS task: services are being analyzed whether they have email functionality</li></ul>OneTick:<ul><li>changes for AIX were tested, waiting for prod information from Quik</li><li>fixing new version can not connect to database </li></ul>EMIR/REFIT:<ul><li>More reqs needed</li><li>RR related task to be discussed</li></ul>RegReporting<ul><li>Sorted out major mess at UK, also at UAT, started to fix EP env, analysis is done, plan meeting with A.Vyugovsky to clarify</li><li>Preparing architecture diagram</li></ul> | 
| top 3-5 points | 
| 1) По проекту Рег Репортинга узнал, что появилось много новых задач по доработкам на РР. И тут много проблем

1.1) они не были запланированы  - cds хотели закрыть, но не закрыты. ресурсы не оценивали. 

1.2) они сложны по сути, а аналитика по системе нет.

1.3) По сроку можем и скорее всего не успеем. Спросил что делать будем, сказали неправильно репортить,

1.4) Статуса проекта сейчас как такового нет. Дима Суздалев в этой роли новый и что и как делать не знает. Задачи заведены, но только те, что в работе. Понять что еще осталось делать сейчас никак нельзя

1.5) Женя М. спрашивала про ресурс Аналитика на Рег репортинг. Ответил, что сейчас нет и это только в далеком будущем. Плохо. Такого ресурса сейчас очень не хватает



2) Сейчас самое критичное - Разработчик на Атриум. Именно в текущий момент предложений нет, собесы не назначены. 

Просто для рассуждения мысль - дешевле было бы Колю оставить, даже за те деньги как он получил в ВТБ. Сейчас потеряем время и проект задержим.



3) В прошлом году в 4ом квартале обсуждали 100500 проблем по ФХ, которые надо решать. Поговорили, обратной связи не было. Так не правильно. Проблемы есть, решения нет, обратной связи нет.

По ФХ вообще надо что то делать... все про проблемы говорят, они не решаются. дальше все это забывают и все по новой

3.1) Что с Менялкой ? Когда погасим или в Банк сдадим ?

 **Последняя сделка в системе - 27-11-2022** 

3.2) Отчет для Финама - закончилось ничем

3.3) Диф курсы для Ибсо - делали и на стороне банка изменились приоритеты. Недоделали.



4)  **!!!!**  Почти заполнил таблицу как я ее вижу по информации и ДР решению по Калипсо. Надо рассмотреть на звонке, согласовать и далее так по всем заполнять → [[Calypso|Calypso]]

5)  **!!!!**  Обучение 2024. Надо выяснить, какие бюджеты на обучение нам по итогу согласовали. Я за 3 года обучения в компании не видел. У всех большие ожидания по этой теме.

6)  **!!!!**  Пример пустой траты ресурса ИТ со стороны ИТ. Работали над этим пол года. [REQ-1738 BCS IB JIRA](https:///browse/REQ-1738)





 | 
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

<ul><li>Из проектов работаем над задачами: Setup BCSCY in Calypso Non UK, CASS</li></ul><ul><li>CASS - исправили проблему по автосетелменту сделок для BCSCY</li><li>BCSCY - сделали сетап ОТС equity option, делали правки по SWIFT инструктированию + неттинг конфо.</li><li>BCSGL - были сделаны донастройки конфигурации в TSL по сделкам, которые есть на PRODCY</li><li>Развернули локально новый инстанс Calypso 17 на NV в UK, чтобы на нем провести регрессионное тестирование текущего функционала. </li></ul>IBQ:

<ul><li>Продолжаем делать аналитику по проекту EMIR Refit. Делаем разработку по формированию файлов EMIR c Trade Report по описанным продуктам. Сделали багфиксинг мелких проблем прода + пара SR-ов к релизу.</li><li>Новый аналитик на аутсорс закончил заниматься задачами на OneTick и переключается на задачу по загрузке данных из Anna DSB для EMIR Refit.</li><li>В праздники сломались диски на сервере, где располагался application QORT ТЧК, сейчас сервер восстановили, занимаемся восстановлением тестового контура QORT.</li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>UK ESB Upgrade: properties and master-lock</li><li>Backlog tasks</li><li>integration with RJOB portal</li></ul>Kondor
1.  **Ресурсная проблема создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Систематика заявила, что они остаются при своем мнении по требованиям к HW, а значит не могут гарантировать заявленной производительности Атриума.
1. В релизе 12.01.24 запланирован вывод задачи по обогащению post-trade репортинга (давно запрошено комплаенсом), а также переключаемся на nonUK почтовый сервер.
1. Получены новые требования по проекту выпуска нот на Казахстане - обработка FX Spot сделок.

 **CRM** 1) Migration of UK CRM service:<ul><li>Migration of metadata ongoing</li><li>Discussing and justifying plan dates for UK PMO</li><li>Request for prolongation of old ogr for 12 days was sent to UK Salesforce - pending answer</li><li>Invoice for new UK org was paid</li></ul>2) MRRA separation on EMIR & SFTR agreement types - separated Agreement types on TEST, provided TEST data to colleagues from EDW3) Full CY clientbase upload & support in CRM - Preparatiopn of full list of required data with format and comments4) Hotifx for UK users rights in old org: making them independant from non-UK sales users approval's on work with client baseRiskroom:<ul><li>SR for FX room delivered to production</li><li>FI related SR is in development and analysis</li></ul>FX:<ul><li>Dev continues for banded tariffication, delployed to UAT, procedural API for bank agreed, testing starting</li><li>Investigate deadlock issue: need to fix WeekendRates service to set transaction level - Snapshot</li><li>EWS task: services are being analyzed whether they have email functionality</li></ul>OneTick:<ul><li>changes for AIX were tested, waiting for prod information from Quik</li><li>fixing new version can not connect to database </li></ul>EMIR/REFIT:<ul><li>More reqs needed</li><li>RR related task to be discussed</li></ul>RegReporting<ul><li>Sorted out major mess at UK, also at UAT, started to fix EP env, analysis is done, plan meeting with A.Vyugovsky to clarify</li><li>Preparing architecture diagram</li></ul> | 
| top 3-5 points | 
| 1) По проекту Рег Репортинга узнал, что появилось много новых задач по доработкам на РР. И тут много проблем

1.1) они не были запланированы  - cds хотели закрыть, но не закрыты. ресурсы не оценивали. 

1.2) они сложны по сути, а аналитика по системе нет.

1.3) По сроку можем и скорее всего не успеем. Спросил что делать будем, сказали неправильно репортить,

1.4) Статуса проекта сейчас как такового нет. Дима Суздалев в этой роли новый и что и как делать не знает. Задачи заведены, но только те, что в работе. Понять что еще осталось делать сейчас никак нельзя

1.5) Женя М. спрашивала про ресурс Аналитика на Рег репортинг. Ответил, что сейчас нет и это только в далеком будущем. Плохо. Такого ресурса сейчас очень не хватает



2) Сейчас самое критичное - Разработчик на Атриум. Именно в текущий момент предложений нет, собесы не назначены. 

Просто для рассуждения мысль - дешевле было бы Колю оставить, даже за те деньги как он получил в ВТБ. Сейчас потеряем время и проект задержим.



3) В прошлом году в 4ом квартале обсуждали 100500 проблем по ФХ, которые надо решать. Поговорили, обратной связи не было. Так не правильно. Проблемы есть, решения нет, обратной связи нет.

По ФХ вообще надо что то делать... все про проблемы говорят, они не решаются. дальше все это забывают и все по новой

3.1) Что с Менялкой ? Когда погасим или в Банк сдадим ?

 **Последняя сделка в системе - 27-11-2022** 

3.2) Отчет для Финама - закончилось ничем

3.3) Диф курсы для Ибсо - делали и на стороне банка изменились приоритеты. Недоделали.



4)  **!!!!**  Почти заполнил таблицу как я ее вижу по информации и ДР решению по Калипсо. Надо рассмотреть на звонке, согласовать и далее так по всем заполнять → [[Calypso|Calypso]]

5)  **!!!!**  Обучение 2024. Надо выяснить, какие бюджеты на обучение нам по итогу согласовали. Я за 3 года обучения в компании не видел. У всех большие ожидания по этой теме.

6)  **!!!!**  Пример пустой траты ресурса ИТ со стороны ИТ. Работали над этим пол года. [REQ-1738 BCS IB JIRA](https:///browse/REQ-1738)





 | 







*****

[[category.storage-team]] 
[[category.confluence]] 
