





| CHG

 | 
| Alexey

 | 
| 

 | 
| Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - делаем разработку по FX Netting Confirmation, работаем над брокерским отчетом. Предоставили примеры CASS сделок для ОХД. Провели демо по CFD.</li><li>BCSGL - сетапили новый продукт депозит, FX в TSL. Исправляли баги.</li><li>BCSUK - баг фиксинг по текущим проблемам прода</li></ul>IBQ: Продолжаем делать аналитику и разработку по проекту EMIR Refit. 

Кондор
1.  **Ресурсная проблема отсутствия разработчика создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Принято решение о выводе интеграции с ТОМС, есть согласование Жени Михайловой и Оли Дудолиной, ожидаем согласования Димы Тренина. Несмотря на всю скудость проведенного бизнес тестирования.
1. Продолжаем вести переговоры с OpenTRM по outsource, получили от них предложение, которое пока не вписывается в наш бюджет.
1. ТЗ Систематики - сократили список открытых вопросов, договорились о начале работ по разработке CW с целью наискорейшего портирования их в наши тестовые системы.

Riskroom:<ul><li>ArmRm - waiting for users feedback</li><li>qkCurrencyRate function replacement for UK - deployed, also found new possible dependency: eqr.pEquityReportMonitor_Calculate<ul><li>found new qk function to migrate: qkSecurities - in progress</li></ul></li><li>CMA room enhancements for CDS portfolio calc for Emir/refit - new REQ for review - in progress</li></ul>FX:<ul><li>Database migration for MABI and Mayalka is plannes this weekend, have to update 2 services - done</li><li>Still having of time requests to database from ntpro2db</li><li>Weekendrates service - fixed a bug updating markups, deployed to prod</li><li>Banded tariffication to plan installation to prod</li><li>Unusual client activity alarm is at prod</li><li>DynRep discussed and waiting for reqs to be ready</li></ul>OneTick, SFTR:<ul><li>SL3 issues</li><li>to plan new SR (qustionnarie)</li></ul>EMIR/REFIT:<ul><li>Oleg/Stas are working on the tasks</li><li>Igor finished working on UTI generation task at IBQ, passed to testing</li></ul>RegReporting<ul><li>List of services reviewed</li><li>To be architecture draft is done - to enhance further</li></ul>EDW<ul><li>Incident with KHD missing prices: workaround applied</li><li>Emir-Refit margin report functionality is testing</li><li>Anna DSB files upload in progress</li><li>FIRS data load is in progress</li><li>Test activities support required to fix Qort load</li><li>to plan new SR (qustionnarie)</li><li>Dmitry Lidvanskiy joined</li></ul>

 | 
| top 3-5 points | 
| 1) По проекту Марекс высоковероятно не успеем реализовать решение по части ОТик - нет постановки, уточняем требования. Желаемый срок окончания - 01-04-24, скорее всего его не сможем удовлетворить. Надо отдельно проговорить с СОО2) По выводу в бой шлюза с ТОМС на Кипре - нужен ОК от Димы Тренина. см. п Кондор.  | 
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

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - делаем разработку по FX Netting Confirmation, работаем над брокерским отчетом. Предоставили примеры CASS сделок для ОХД. Провели демо по CFD.</li><li>BCSGL - сетапили новый продукт депозит, FX в TSL. Исправляли баги.</li><li>BCSUK - баг фиксинг по текущим проблемам прода</li></ul>IBQ: Продолжаем делать аналитику и разработку по проекту EMIR Refit. 

Кондор
1.  **Ресурсная проблема отсутствия разработчика создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Принято решение о выводе интеграции с ТОМС, есть согласование Жени Михайловой и Оли Дудолиной, ожидаем согласования Димы Тренина. Несмотря на всю скудость проведенного бизнес тестирования.
1. Продолжаем вести переговоры с OpenTRM по outsource, получили от них предложение, которое пока не вписывается в наш бюджет.
1. ТЗ Систематики - сократили список открытых вопросов, договорились о начале работ по разработке CW с целью наискорейшего портирования их в наши тестовые системы.

Riskroom:<ul><li>ArmRm - waiting for users feedback</li><li>qkCurrencyRate function replacement for UK - deployed, also found new possible dependency: eqr.pEquityReportMonitor_Calculate<ul><li>found new qk function to migrate: qkSecurities - in progress</li></ul></li><li>CMA room enhancements for CDS portfolio calc for Emir/refit - new REQ for review - in progress</li></ul>FX:<ul><li>Database migration for MABI and Mayalka is plannes this weekend, have to update 2 services - done</li><li>Still having of time requests to database from ntpro2db</li><li>Weekendrates service - fixed a bug updating markups, deployed to prod</li><li>Banded tariffication to plan installation to prod</li><li>Unusual client activity alarm is at prod</li><li>DynRep discussed and waiting for reqs to be ready</li></ul>OneTick, SFTR:<ul><li>SL3 issues</li><li>to plan new SR (qustionnarie)</li></ul>EMIR/REFIT:<ul><li>Oleg/Stas are working on the tasks</li><li>Igor finished working on UTI generation task at IBQ, passed to testing</li></ul>RegReporting<ul><li>List of services reviewed</li><li>To be architecture draft is done - to enhance further</li></ul>EDW<ul><li>Incident with KHD missing prices: workaround applied</li><li>Emir-Refit margin report functionality is testing</li><li>Anna DSB files upload in progress</li><li>FIRS data load is in progress</li><li>Test activities support required to fix Qort load</li><li>to plan new SR (qustionnarie)</li><li>Dmitry Lidvanskiy joined</li></ul>

 | 
| top 3-5 points | 
| 1) По проекту Марекс высоковероятно не успеем реализовать решение по части ОТик - нет постановки, уточняем требования. Желаемый срок окончания - 01-04-24, скорее всего его не сможем удовлетворить. Надо отдельно проговорить с СОО2) По выводу в бой шлюза с ТОМС на Кипре - нужен ОК от Димы Тренина. см. п Кондор.  | 







*****

[[category.storage-team]] 
[[category.confluence]] 
