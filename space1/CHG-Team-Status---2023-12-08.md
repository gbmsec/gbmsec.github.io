





| CHG

 | 
| Alexey

 | 
| 

 | 
| Кондор 
1. Олейник (разработчик) проходит СБ.
1. QA протестировали наше решение по возможности отключения UK экспортера. Планируем вывод в релизе 16.12.
1. Выводим внеплановым релизом 08.12 доработку, позволяющую передавать ОТС сделки Казахстана в nonUK Калипсо.
1. Поменяли архитектуру фильтрации загрузки с NT-Pro - теперь на нашей стороне.
1. По запросу МО отключили из загрузки несколько десятков счетов.



ESB

<ul><li>ESB internal tasks and bugs</li><li>ESB mails via EWS Cloud</li><li>UK ActiveMQ → Artemis migration</li><li>TOMS EP</li></ul>

Calypso:

<ul><li>Из проектов работаем над задачами: Setup BCSCY in Calypso Non UK, CASS</li></ul><ul><li>CASS - продолжаем тестирование и багфиксинг по реализованным продуктам. Ждем проведение UAT по CMAR отчету.</li><li>BCSCY - Делаем доработки по Trade Confirmation и Agency Repo. Также настраиваем сетап продуктов по CDS (RO, Basket, Loan)</li><li>Запуск Calypso PRODCY  </li></ul>IBQ:

<ul><li>Продолжаем делать аналитику по проекту EMIR Refit. Делаем разработку по формированию файлов EMIR c Trade Report по описанным продуктам. </li><li>C коллегами из БКС Россия делаем тестирование по сделкам и предоставлению им нужного пакета документов для запуска сверок в автоматическом режиме. Есть вопросы по нумерации сделок, в BO сделка имеет постфикс /1, что отличается от номера который предоставляет Кондор.</li><li>Вышел новый аналитик на аутсорс, запрашиваем ему доступ на OneTick, а также предоставляем ему экспертизу по данному сервису.</li><li> Вывод релиза QORT</li></ul>Riskroom: 2 SR to evaluate FX: Dev started for banded tarifficationOneTick: Started discussion with testing team on setting up env to test All AIX changes at UATEMIR/REFIT: Dev is ongoingRegReporting<ul><li>Ready to move UK database</li><li>Found massive mess with REGT services at UK, still sorting out to complete moving to another db:<ul><li>Sanctions Control steals messages</li><li>FileMonitor does not work</li></ul></li><li>Preparing architecture diagram</li></ul>Candidates:<ul><li>onboarding Stas Tagiev (parttime)</li><li>waiting Igor Beloshapka to start 11/12</li></ul> | 
| top 3-5 points | 
|  **Вопрос к ОПС** : SWIFT'ы для CY IBQ до сих пор продолжают приходить через UK Autoclient | 
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
| Кондор 
1. Олейник (разработчик) проходит СБ.
1. QA протестировали наше решение по возможности отключения UK экспортера. Планируем вывод в релизе 16.12.
1. Выводим внеплановым релизом 08.12 доработку, позволяющую передавать ОТС сделки Казахстана в nonUK Калипсо.
1. Поменяли архитектуру фильтрации загрузки с NT-Pro - теперь на нашей стороне.
1. По запросу МО отключили из загрузки несколько десятков счетов.



ESB

<ul><li>ESB internal tasks and bugs</li><li>ESB mails via EWS Cloud</li><li>UK ActiveMQ → Artemis migration</li><li>TOMS EP</li></ul>

Calypso:

<ul><li>Из проектов работаем над задачами: Setup BCSCY in Calypso Non UK, CASS</li></ul><ul><li>CASS - продолжаем тестирование и багфиксинг по реализованным продуктам. Ждем проведение UAT по CMAR отчету.</li><li>BCSCY - Делаем доработки по Trade Confirmation и Agency Repo. Также настраиваем сетап продуктов по CDS (RO, Basket, Loan)</li><li>Запуск Calypso PRODCY  </li></ul>IBQ:

<ul><li>Продолжаем делать аналитику по проекту EMIR Refit. Делаем разработку по формированию файлов EMIR c Trade Report по описанным продуктам. </li><li>C коллегами из БКС Россия делаем тестирование по сделкам и предоставлению им нужного пакета документов для запуска сверок в автоматическом режиме. Есть вопросы по нумерации сделок, в BO сделка имеет постфикс /1, что отличается от номера который предоставляет Кондор.</li><li>Вышел новый аналитик на аутсорс, запрашиваем ему доступ на OneTick, а также предоставляем ему экспертизу по данному сервису.</li><li> Вывод релиза QORT</li></ul>Riskroom: 2 SR to evaluate FX: Dev started for banded tarifficationOneTick: Started discussion with testing team on setting up env to test All AIX changes at UATEMIR/REFIT: Dev is ongoingRegReporting<ul><li>Ready to move UK database</li><li>Found massive mess with REGT services at UK, still sorting out to complete moving to another db:<ul><li>Sanctions Control steals messages</li><li>FileMonitor does not work</li></ul></li><li>Preparing architecture diagram</li></ul>Candidates:<ul><li>onboarding Stas Tagiev (parttime)</li><li>waiting Igor Beloshapka to start 11/12</li></ul> | 
| top 3-5 points | 
|  **Вопрос к ОПС** : SWIFT'ы для CY IBQ до сих пор продолжают приходить через UK Autoclient | 







*****

[[category.storage-team]] 
[[category.confluence]] 
