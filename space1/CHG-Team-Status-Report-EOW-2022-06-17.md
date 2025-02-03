





| CHG

 | 
| Alexey Dorogov

 | 
|    

 | 
| Business monitoring implemented for CY perimiter - [http://dcix-sqlmon01:3000/d/78BA7wj7z/cy-business-activity?orgId=1&refresh=15m](http://dcix-sqlmon01:3000/d/78BA7wj7z/cy-business-activity?orgId=1&refresh=15m)Calypso<ul><li>Продолжаем заниматься приоритетными задачами по проекту FAB и CASS. </li><li>Провели оценку по задачам для открытия проекта S-Accounts</li></ul>CRM1) Calypso full scale integration - по результатам предоставления данных коллеги вернули комментарии и пожелания. Они были учтены, внесены правки в интеграция и новая тестовая выгрузка была предоставлена 2) LEI Expiry autoupdate - уведомления об истечении LEI переведены в формат единого отчета, рассылка запущена с 13 июня. Задача полностью реализована 3) User turn down improved process - выведен в прод процесс отключения пользователя (максимально возможная автоматизация сбора данных для модификации и минимизация ошибок из-за человеческого фактора) 4) Next Ongoing KYC Review FIX - найден и исправлен редкий сценарий, когда дата следующей плановой проверки KYC обновлялась некорректно в случае перевода клиента/контрагента в статус Terminated и последующем возвращении его в Live. 5) Conga Courier rebuild with Conga Composer+Batch - переход со старой схемы вендорского продукта для гибкой отправки отчётов (более не поддерживаемой) на новую был осуществленEDW<ul><li>SCS NRD data check</li><li>EMIR reconciliation</li></ul>Kondor
1. Казначейство занялось "обнулением" позиций. Пока не произошло, но, по крайней мере, пишут письма и задают какие-то вопросы, мы пытаемся отвечать.
1. Актуализированы Action Plan-ы проблем, одна закрыта.
1. Проведен мозговой штурм по ведению книжек в К+, вышли на КХД, запланировали встречу.
1. На high-level оценили  [PRJ-290](http://jira/browse/PRJ-290) - C-accounts: trading on moex for non-residents  **ANALYSIS**   (S-accounts: trading on moex for non-residents)

RRSprint planned. Backlog is cleaned up. Ready to migrate from Risk_In to RiskNew_In - old tech debt for integration improvementFX
1. На этой неделе пришла проверка ЦБ в банк, всю неделю занимались этим вопросом. Были подготовлены данные по отдаваемым котировкам в системы БКС Онлайн, Менялка, Менялка (Приложение), Corporates начиная с 01.03.2022. 
1. Разбирали вопросы связанные с увеличением количества перекрытых в НТ сделок отвергнутых ИБСО 

ESB<ul><li>ESB Migration to Kubernetes. Reports</li><li>BCSBroker reports parser for IBQ</li><li>ESB Migration to Kubernetes. MailTransfer bugs</li></ul> | 
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
| Alexey Dorogov

 | 
|    

 | 
| Business monitoring implemented for CY perimiter - [http://dcix-sqlmon01:3000/d/78BA7wj7z/cy-business-activity?orgId=1&refresh=15m](http://dcix-sqlmon01:3000/d/78BA7wj7z/cy-business-activity?orgId=1&refresh=15m)Calypso<ul><li>Продолжаем заниматься приоритетными задачами по проекту FAB и CASS. </li><li>Провели оценку по задачам для открытия проекта S-Accounts</li></ul>CRM1) Calypso full scale integration - по результатам предоставления данных коллеги вернули комментарии и пожелания. Они были учтены, внесены правки в интеграция и новая тестовая выгрузка была предоставлена 2) LEI Expiry autoupdate - уведомления об истечении LEI переведены в формат единого отчета, рассылка запущена с 13 июня. Задача полностью реализована 3) User turn down improved process - выведен в прод процесс отключения пользователя (максимально возможная автоматизация сбора данных для модификации и минимизация ошибок из-за человеческого фактора) 4) Next Ongoing KYC Review FIX - найден и исправлен редкий сценарий, когда дата следующей плановой проверки KYC обновлялась некорректно в случае перевода клиента/контрагента в статус Terminated и последующем возвращении его в Live. 5) Conga Courier rebuild with Conga Composer+Batch - переход со старой схемы вендорского продукта для гибкой отправки отчётов (более не поддерживаемой) на новую был осуществленEDW<ul><li>SCS NRD data check</li><li>EMIR reconciliation</li></ul>Kondor
1. Казначейство занялось "обнулением" позиций. Пока не произошло, но, по крайней мере, пишут письма и задают какие-то вопросы, мы пытаемся отвечать.
1. Актуализированы Action Plan-ы проблем, одна закрыта.
1. Проведен мозговой штурм по ведению книжек в К+, вышли на КХД, запланировали встречу.
1. На high-level оценили  [PRJ-290](http://jira/browse/PRJ-290) - C-accounts: trading on moex for non-residents  **ANALYSIS**   (S-accounts: trading on moex for non-residents)

RRSprint planned. Backlog is cleaned up. Ready to migrate from Risk_In to RiskNew_In - old tech debt for integration improvementFX
1. На этой неделе пришла проверка ЦБ в банк, всю неделю занимались этим вопросом. Были подготовлены данные по отдаваемым котировкам в системы БКС Онлайн, Менялка, Менялка (Приложение), Corporates начиная с 01.03.2022. 
1. Разбирали вопросы связанные с увеличением количества перекрытых в НТ сделок отвергнутых ИБСО 

ESB<ul><li>ESB Migration to Kubernetes. Reports</li><li>BCSBroker reports parser for IBQ</li><li>ESB Migration to Kubernetes. MailTransfer bugs</li></ul> | 
| top 3-5 points | 
|  | 







*****

[[category.storage-team]] 
[[category.confluence]] 
