





| CHG

 | 
| Alexey

 | 
| 

 | 
| ESB

<ul><li>ESB internal tasks and bugs</li><li>UK. ESB Upgrade: camel version</li><li>UK. Migration Activemq → ArtemisMQ</li><li>EP. BCSGL statements processing</li></ul>

Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - тестирование функционала на новой версии Calypso 17. Проверили OPS Statistic Report + сделали доработку по сетелменту CASS.</li><li>BCSGL - тестирование функционала на новой версии Calypso 17. Делали доработки по TSL по новым продуктам. Сделали загрузку внешних выписок для сверок по брокерам BCSRU, BCSCY, RBC.</li><li>BCSUK - исправили ошибки по Position Keeper по CA.</li><li>Закончили тестирование инстансов Calypso 17 на Кипре PREPCY17 и UATCY17. Получили аппрув на вывод в PROD.</li><li>Провели планирование задач на новый спринт</li><li>Вывод релизов CY и UK   В рамках релиза CY выводится новая 17 версия Калипсо.</li></ul>IBQ: Продолжаем делать аналитику и разработку по проекту EMIR Refit. 

Riskroom:<ul><li>ArmRm - AVG volumes for risk category is done</li><li>qkCurrencyRate function replacement for UK - testing in progress, also found new possible dependency: eqr.pEquityReportMonitor_Calculate<ul><li>found new qk function to migrate: qkSecurities</li></ul></li><li>CMA room enhancements for CDS portfolio calc for Emir/refit - new REQ for review</li></ul>FX:<ul><li>Database migration for MABI and Mayalka is plannes this weekend, have to update 2 services</li><li>Weekendrates service - fixed a bug updating markups. UAT, deployed</li><li>Banded tariffication testing started</li><li>Unusual client activity alarm is at UAT</li><li>DynRep discussed and waiting for reqs to be ready</li><li>New functionality is ready, preparing to deploy</li></ul>OneTick, SFTR:<ul><li>SL3 issues</li></ul>EMIR/REFIT:<ul><li>Oleg/Stas are working on the tasks</li><li>Igor finished working on UTI generation task at IBQ, passed to testing</li></ul>RegReporting<ul><li>List of services reviewed</li><li>To be architecture draft is done</li></ul>EDW<ul><li>Emir-Refit margin report functionality is testing</li><li>Anna DSB files upload in progress</li><li>FIRS data load is in progress</li><li>Test activities support required to fix Qort load</li><li>Dmitry Lidvanskiy joins next Monday</li></ul>Kondor
1.  **Ресурсная проблема отсутствия разработчика создает огромные риски для проекта перехода на Атриум в этом году.** 
1. КПИ команды на 2024 - переход на Атриум. Занесен в список.
1. Проведен UAT интеграции Атриума с Калипсо по LE.
1. Предложено изменение ведения описания функционала - не на основе системы, а как МО - далее Атриум.
1. Проведены консультации с новым рекрутером. Еще раз подчеркнул, что упор надо делать на разработчика.
1. Ведем согласование списка задач с OpenTRM (возможный outsource на проекте перехода на Атриум)

 | 
| top 3-5 points | 
| 1) возможен вывод сотрудника на EDW  в понедельник2) Был звонок по РегРепортингу. Обсуждали срочные задачи. сть много РЕК, которые надо делать. Делать некем. РегТим скоммуницировал срок реализации как март,24. Обсудили, что срок не правильный. Надо исправлять срок.!!! Составлен список задач по доработкам РегРепортинга. Список в письме. 8 РЕК в нем. Список большой, заниматься некому. На 80% доработки по SFTR.3) Допник с новыми сроками для Калипсо подписали.4) Информации по ценам и ставкам на вендоров от Группы нет. ВДКом уже спрашивает про продление договора. Надо готовить новый допник.5) Выявлен и обсудили с коллегами на звонке по регРепортингу случай, когда регистрируют РЕК с доработками на кучу систем. Все согласовали. Я специально обращаю внимание - надо сказать всем на вашей встрече, что такие РЕК не надо регистрировать - надо либо проект, либо подтверждение, что им будет управлять заказчик и координировать все доработки. REQ-2033. 6) Провели звонок и направил Максиму Архитектуру по РегРепортинку Кипра.7) Обсудил с Росаной тему веб-сайта BCSGM. Росана согласна, что надо переделывать сайт. Создала чат в Рокете, где обратилась к Тимуру с вопросам чем будем наполнять. Тимур ничего не ответил и вопрос встал. Я хочу собрать пожелания и с Денисом в течение года найти фреймворк под статический сайт и сделать на базе него наш новый, наполнив актуальной информацией.8) Где информация по бонусам и переоценкам ЗП ? уже март начался9) В файле с БД Оракл отметили те которые нам не нужны. Есть в списке 2 Бд больших размеров. | 
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
| ESB

<ul><li>ESB internal tasks and bugs</li><li>UK. ESB Upgrade: camel version</li><li>UK. Migration Activemq → ArtemisMQ</li><li>EP. BCSGL statements processing</li></ul>

Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - тестирование функционала на новой версии Calypso 17. Проверили OPS Statistic Report + сделали доработку по сетелменту CASS.</li><li>BCSGL - тестирование функционала на новой версии Calypso 17. Делали доработки по TSL по новым продуктам. Сделали загрузку внешних выписок для сверок по брокерам BCSRU, BCSCY, RBC.</li><li>BCSUK - исправили ошибки по Position Keeper по CA.</li><li>Закончили тестирование инстансов Calypso 17 на Кипре PREPCY17 и UATCY17. Получили аппрув на вывод в PROD.</li><li>Провели планирование задач на новый спринт</li><li>Вывод релизов CY и UK   В рамках релиза CY выводится новая 17 версия Калипсо.</li></ul>IBQ: Продолжаем делать аналитику и разработку по проекту EMIR Refit. 

Riskroom:<ul><li>ArmRm - AVG volumes for risk category is done</li><li>qkCurrencyRate function replacement for UK - testing in progress, also found new possible dependency: eqr.pEquityReportMonitor_Calculate<ul><li>found new qk function to migrate: qkSecurities</li></ul></li><li>CMA room enhancements for CDS portfolio calc for Emir/refit - new REQ for review</li></ul>FX:<ul><li>Database migration for MABI and Mayalka is plannes this weekend, have to update 2 services</li><li>Weekendrates service - fixed a bug updating markups. UAT, deployed</li><li>Banded tariffication testing started</li><li>Unusual client activity alarm is at UAT</li><li>DynRep discussed and waiting for reqs to be ready</li><li>New functionality is ready, preparing to deploy</li></ul>OneTick, SFTR:<ul><li>SL3 issues</li></ul>EMIR/REFIT:<ul><li>Oleg/Stas are working on the tasks</li><li>Igor finished working on UTI generation task at IBQ, passed to testing</li></ul>RegReporting<ul><li>List of services reviewed</li><li>To be architecture draft is done</li></ul>EDW<ul><li>Emir-Refit margin report functionality is testing</li><li>Anna DSB files upload in progress</li><li>FIRS data load is in progress</li><li>Test activities support required to fix Qort load</li><li>Dmitry Lidvanskiy joins next Monday</li></ul>Kondor
1.  **Ресурсная проблема отсутствия разработчика создает огромные риски для проекта перехода на Атриум в этом году.** 
1. КПИ команды на 2024 - переход на Атриум. Занесен в список.
1. Проведен UAT интеграции Атриума с Калипсо по LE.
1. Предложено изменение ведения описания функционала - не на основе системы, а как МО - далее Атриум.
1. Проведены консультации с новым рекрутером. Еще раз подчеркнул, что упор надо делать на разработчика.
1. Ведем согласование списка задач с OpenTRM (возможный outsource на проекте перехода на Атриум)

 | 
| top 3-5 points | 
| 1) возможен вывод сотрудника на EDW  в понедельник2) Был звонок по РегРепортингу. Обсуждали срочные задачи. сть много РЕК, которые надо делать. Делать некем. РегТим скоммуницировал срок реализации как март,24. Обсудили, что срок не правильный. Надо исправлять срок.!!! Составлен список задач по доработкам РегРепортинга. Список в письме. 8 РЕК в нем. Список большой, заниматься некому. На 80% доработки по SFTR.3) Допник с новыми сроками для Калипсо подписали.4) Информации по ценам и ставкам на вендоров от Группы нет. ВДКом уже спрашивает про продление договора. Надо готовить новый допник.5) Выявлен и обсудили с коллегами на звонке по регРепортингу случай, когда регистрируют РЕК с доработками на кучу систем. Все согласовали. Я специально обращаю внимание - надо сказать всем на вашей встрече, что такие РЕК не надо регистрировать - надо либо проект, либо подтверждение, что им будет управлять заказчик и координировать все доработки. REQ-2033. 6) Провели звонок и направил Максиму Архитектуру по РегРепортинку Кипра.7) Обсудил с Росаной тему веб-сайта BCSGM. Росана согласна, что надо переделывать сайт. Создала чат в Рокете, где обратилась к Тимуру с вопросам чем будем наполнять. Тимур ничего не ответил и вопрос встал. Я хочу собрать пожелания и с Денисом в течение года найти фреймворк под статический сайт и сделать на базе него наш новый, наполнив актуальной информацией.8) Где информация по бонусам и переоценкам ЗП ? уже март начался9) В файле с БД Оракл отметили те которые нам не нужны. Есть в списке 2 Бд больших размеров. | 







*****

[[category.storage-team]] 
[[category.confluence]] 
