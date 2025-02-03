





| CHG

 | 
| Alexey

 | 
| 

 | 
| Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - Занимаемся анализом продукта CFD и изучили его реализацию в ритейле. Тестируем загрузку биржевых сделок по Кипру и созданию ноги на Казахстан. Продолжаем анализ по доработкам брокерского отчета. Тестируем продуктовую интеграцию с ОХД. Делаем анализ по MiFID Transaction Reporting.</li><li>BCSGL - ждем требования на сетпа FX продукта для Казахстана и его обработку в TSL. Занимаемся доработкой сверок для брокеров BCSRU и BCSCY.</li><li>BCSUK - предоставили ответы по обработке CA сделок и трансфер агентов по Funding UK. Реализовали таски по автоматической загрузке LAW и RES списков.</li><li>Провели первую встречу с аудиторами CUSIP по поводу загрузки данных из Bloomberg. С нашей стороны необходимо нарисовать техническую схему и предоставить описание текущего процесса. Следующая встреча запланирована на  </li><li>Тестируем локально развернутый новый инстанс Calypso 17 на NV ресурсом QA. Приняли решение на обновление тестовых сред Кипра на 17 версию после релиза  Сделали сохранение тестовых данных с PREPCY для загрузки в 17 версию PREPCY17.</li></ul>IBQ:

<ul><li>Продолжаем делать аналитику по проекту EMIR Refit. Делаем разработку по настройке расписания запуска отчетов и исправлением системных багов и конфликтов.</li></ul>

Кондор
1.  **Ресурсная проблема отсутствия разработчика создает огромные риски для проекта перехода на Атриум в этом году.** 
1. По найму Крадетской принято отрицательное решение. И снова поиск... При том, что меняется рекрутер (причем новый пока в отпуске).
1. Релиз перенесен на следующую неделю из-за тестирования инфраструктурного DR. Ну а сами принимаем участие в тестировании.
1. По косвенным признакам можно судить, что Систематика вступила в активную фазу работ у нас на сайте. Был от них звонок, где они сказали, что им мало одной ноды для доступа. Проинформировал, что нод выделено 3.
1. Начали строить тестовое интеграционное окружение для Атриума. Первым шагом идет шина и Калипсо (можно тестировать загрузку контрагентов и клиентов).
1. !!! Принято решение о переносе транспорта сплитов в КХД в этом году.

Riskroom:<ul><li>ArmRm - intraday utilization report is in prod, also VG made some test cases at UAT</li><li>qkCurrencyRate function replacement for UK is ready, test prepared and planned for Monday</li><li>Working on CMA room enhancements for CDS portfolio calc for Emir/refit</li></ul>FX:<ul><li>Weekendrates service - found some bug updating markups</li><li>DB SQL timeout problem arises at NtPro, need to migrate to another server - still to be planned</li><li>Banded tariffication agreed on using our view with log option</li><li>Started to implement Unusual client activity alarm</li><li>DynRep discussed</li></ul>EMIR/REFIT: RR related task (CMA room) - implementation startedRegReporting - Fixed SC service problemEDW<ul><li>KT from Alexander Kravchenko</li><li>1 interview</li></ul> | 
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

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - Занимаемся анализом продукта CFD и изучили его реализацию в ритейле. Тестируем загрузку биржевых сделок по Кипру и созданию ноги на Казахстан. Продолжаем анализ по доработкам брокерского отчета. Тестируем продуктовую интеграцию с ОХД. Делаем анализ по MiFID Transaction Reporting.</li><li>BCSGL - ждем требования на сетпа FX продукта для Казахстана и его обработку в TSL. Занимаемся доработкой сверок для брокеров BCSRU и BCSCY.</li><li>BCSUK - предоставили ответы по обработке CA сделок и трансфер агентов по Funding UK. Реализовали таски по автоматической загрузке LAW и RES списков.</li><li>Провели первую встречу с аудиторами CUSIP по поводу загрузки данных из Bloomberg. С нашей стороны необходимо нарисовать техническую схему и предоставить описание текущего процесса. Следующая встреча запланирована на  </li><li>Тестируем локально развернутый новый инстанс Calypso 17 на NV ресурсом QA. Приняли решение на обновление тестовых сред Кипра на 17 версию после релиза  Сделали сохранение тестовых данных с PREPCY для загрузки в 17 версию PREPCY17.</li></ul>IBQ:

<ul><li>Продолжаем делать аналитику по проекту EMIR Refit. Делаем разработку по настройке расписания запуска отчетов и исправлением системных багов и конфликтов.</li></ul>

Кондор
1.  **Ресурсная проблема отсутствия разработчика создает огромные риски для проекта перехода на Атриум в этом году.** 
1. По найму Крадетской принято отрицательное решение. И снова поиск... При том, что меняется рекрутер (причем новый пока в отпуске).
1. Релиз перенесен на следующую неделю из-за тестирования инфраструктурного DR. Ну а сами принимаем участие в тестировании.
1. По косвенным признакам можно судить, что Систематика вступила в активную фазу работ у нас на сайте. Был от них звонок, где они сказали, что им мало одной ноды для доступа. Проинформировал, что нод выделено 3.
1. Начали строить тестовое интеграционное окружение для Атриума. Первым шагом идет шина и Калипсо (можно тестировать загрузку контрагентов и клиентов).
1. !!! Принято решение о переносе транспорта сплитов в КХД в этом году.

Riskroom:<ul><li>ArmRm - intraday utilization report is in prod, also VG made some test cases at UAT</li><li>qkCurrencyRate function replacement for UK is ready, test prepared and planned for Monday</li><li>Working on CMA room enhancements for CDS portfolio calc for Emir/refit</li></ul>FX:<ul><li>Weekendrates service - found some bug updating markups</li><li>DB SQL timeout problem arises at NtPro, need to migrate to another server - still to be planned</li><li>Banded tariffication agreed on using our view with log option</li><li>Started to implement Unusual client activity alarm</li><li>DynRep discussed</li></ul>EMIR/REFIT: RR related task (CMA room) - implementation startedRegReporting - Fixed SC service problemEDW<ul><li>KT from Alexander Kravchenko</li><li>1 interview</li></ul> | 
| top 3-5 points | 
|  | 







*****

[[category.storage-team]] 
[[category.confluence]] 
