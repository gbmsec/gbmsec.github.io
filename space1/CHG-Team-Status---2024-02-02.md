





| CHG

 | 
| Alexey

 | 
| 

 | 
| ESB

<ul><li>ESB internal tasks and bugs</li><li>UK ESB Upgrade: java version</li><li>UK ESB Upgrade: camel version</li><li>UK ESB Upgrade: artemis</li><li>Backlog tasks</li></ul>

Riskroom:

<ul><li>ArmRm - intraday utilization report is ready to deploy</li><li>qkCurrencyRate function replacement for UK is ready, still to test</li><li>Working on CMA room enhancements for CDS portfolio calc for Emir/refit</li></ul>FX:

<ul><li>Weekendrates service db errors are fixed with new version</li><li>DB SQL timeout problem arises at NtPro, need to migrate to another server</li><li>Banded tariffication agreed on using our view with log option</li><li>Started to implement Unusual client activity alarm</li></ul>OneTick: Review new req with Slava

EMIR/REFIT:

<ul><li>One more task went to dev (Margin report), discussion with analyst</li><li>RR related task (CMA room) - implementation started</li></ul>RegReporting

<ul><li>Paused:<ul><li>Continued fixing SC reconciliation service at UK</li><li>Preparing architecture diagram</li></ul></li></ul>EDW

<ul><li>KT from Alexander Kravchenko</li></ul>



Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - делаем доработки по сетелменту, нетингам и баг по RUS UBO. Продолжаем разработку новой формы брокерского отчета для TTCA и CASS клиентов. Продолжаем работы над задачей по Liquidity Report. Делаем ревью полей по MiFID Transaction Reporting. Изучаем как сетапить продукт CFD в Калипсо.</li><li>BCSGL - делаем сверки с БКС Брокером. Продолжаем багфиксинг проблем с TSL, Выкатили хотфикс с исправлением TSL  </li><li>BCSUK - делаем доработки по Instant Liquidity Report. Изучаем баг по которому не происходит корректное изменение трансферов.  </li><li>Тестируем локально развернутый новый инстанс Calypso 17 на NV ресурсом QA. Протестировали загрузку тестовых данных из 16 версии в 17.</li></ul>IBQ:

<ul><li>Продолжаем делать аналитику по проекту EMIR Refit. Делаем разработку по настройке расписания запуска отчетов и исправлением системных багов и конфликтов.</li><li>Вместе с командой RiskRoom обновляем логику загрузки сделок в RR, расчет портфелей контрагентов с учетом нового параметра Collateralisation category, а также настройку выгрузки в EDW EP.</li><li>Новый аналитик на аутсорс, делает выгрузки тестовых данных по OT. Делает анализ по загрузке данных из Anna DSB в EDW для EMIR Refit проекта.</li></ul>kondor
1.  **Ресурсная проблема отсутствия разработчика создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Намечены контуры архитектуры ведения сделок в Атриуме.
1. Запущен процесс по найму Крадетской на позицию аналитика.
1. Поиск по Локатору не дал особых результатов для найма разработчика.
1. КС вовлеклись в процесс разработки по проекту. На первой задаче отлаживаются все тонкости и шероховатости и организуется процесс. Эта задача интеграции экспорта, полностью ее сейчас, без наличия CW, все равно нельзя, но процесс взаимодействия наладить можно.

 | 
| top 3-5 points | 
| === | 
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

<ul><li>ESB internal tasks and bugs</li><li>UK ESB Upgrade: java version</li><li>UK ESB Upgrade: camel version</li><li>UK ESB Upgrade: artemis</li><li>Backlog tasks</li></ul>

Riskroom:

<ul><li>ArmRm - intraday utilization report is ready to deploy</li><li>qkCurrencyRate function replacement for UK is ready, still to test</li><li>Working on CMA room enhancements for CDS portfolio calc for Emir/refit</li></ul>FX:

<ul><li>Weekendrates service db errors are fixed with new version</li><li>DB SQL timeout problem arises at NtPro, need to migrate to another server</li><li>Banded tariffication agreed on using our view with log option</li><li>Started to implement Unusual client activity alarm</li></ul>OneTick: Review new req with Slava

EMIR/REFIT:

<ul><li>One more task went to dev (Margin report), discussion with analyst</li><li>RR related task (CMA room) - implementation started</li></ul>RegReporting

<ul><li>Paused:<ul><li>Continued fixing SC reconciliation service at UK</li><li>Preparing architecture diagram</li></ul></li></ul>EDW

<ul><li>KT from Alexander Kravchenko</li></ul>



Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - делаем доработки по сетелменту, нетингам и баг по RUS UBO. Продолжаем разработку новой формы брокерского отчета для TTCA и CASS клиентов. Продолжаем работы над задачей по Liquidity Report. Делаем ревью полей по MiFID Transaction Reporting. Изучаем как сетапить продукт CFD в Калипсо.</li><li>BCSGL - делаем сверки с БКС Брокером. Продолжаем багфиксинг проблем с TSL, Выкатили хотфикс с исправлением TSL  </li><li>BCSUK - делаем доработки по Instant Liquidity Report. Изучаем баг по которому не происходит корректное изменение трансферов.  </li><li>Тестируем локально развернутый новый инстанс Calypso 17 на NV ресурсом QA. Протестировали загрузку тестовых данных из 16 версии в 17.</li></ul>IBQ:

<ul><li>Продолжаем делать аналитику по проекту EMIR Refit. Делаем разработку по настройке расписания запуска отчетов и исправлением системных багов и конфликтов.</li><li>Вместе с командой RiskRoom обновляем логику загрузки сделок в RR, расчет портфелей контрагентов с учетом нового параметра Collateralisation category, а также настройку выгрузки в EDW EP.</li><li>Новый аналитик на аутсорс, делает выгрузки тестовых данных по OT. Делает анализ по загрузке данных из Anna DSB в EDW для EMIR Refit проекта.</li></ul>kondor
1.  **Ресурсная проблема отсутствия разработчика создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Намечены контуры архитектуры ведения сделок в Атриуме.
1. Запущен процесс по найму Крадетской на позицию аналитика.
1. Поиск по Локатору не дал особых результатов для найма разработчика.
1. КС вовлеклись в процесс разработки по проекту. На первой задаче отлаживаются все тонкости и шероховатости и организуется процесс. Эта задача интеграции экспорта, полностью ее сейчас, без наличия CW, все равно нельзя, но процесс взаимодействия наладить можно.

 | 
| top 3-5 points | 
| === | 







*****

[[category.storage-team]] 
[[category.confluence]] 
