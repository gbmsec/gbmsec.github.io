





| CHG

 | 
| Alexey

 | 
| 

 | 
| Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - доделали Trade Confirmation по продуктам. Тестируем загрузку сделок из QUIK через Exporter.</li><li>BCSGL - в TSL сделали донастройки для нового продукта Bank Deposit</li><li>BCSUK - собрали статистику ISIN-ов в рамках аудит запроса от CUSIP. Сделали мелкий багфиксинг по задачам Лены Баско.</li></ul>

IBQ: Продолжаем делать аналитику и разработку по проекту EMIR Refit. Сделали доработки по двум критичным SR по загрузке неторговый поручений и DVP / RVP сделок

CRM **EMIR REFIT:** 

<ul><li>Web form UI is finalized</li><li>Integrational Selects are changed to contain new fields</li><li>Test data added on sandbox</li></ul> **Service Cloud:** <ul><li>Recieving and analysing setup costs and technical options with current vendor and new CY resser of SF products.</li><li>Asking Salesforce directly for setup options with current CY org</li></ul> **Project K - ** Asked to add 10 MD to our evaluation since new requiments (QI status on CY) appeared **Finalizing current CRM developement pipeline**   **overview** Riskroom:<ul><li>SL3: had to fight with UK database problems consequences; also there was a request to get BBG prices for particular list of ISINs</li><li>ArmRm - meeting with Robert, all seems to be implemented, need feedback from production usage</li><li>qkCurrencyRate function replacement for UK - deployed, qkSecurities dependency eliminated, ready to switch off QUIK</li><li>REQ: CMA room enhancements for CDS portfolio calc for Emir/refit - UAT</li></ul>FX:<ul><li>Still having of time requests to database from ntpro2db - timeout enlarged, implemented to prod, to monitor</li><li>Banded tariffication - installed to prod, working on issues found</li><li>Unusual client activity alarm is at prod, also some minor changed deployed</li><li>DynRep: started to develop, no test data</li><li>News portal: minor changes, also to sort out some users do have some role</li></ul>OneTick, SFTR:<ul><li>OneTick: new release planned for Monday</li><li>Murex project: some minor activities, waiting for analysis</li><li>to plan new SR (qustionnarie) - analysis</li></ul>EMIR/REFIT:<ul><li>Oleg/Stas are working on the tasks</li><li>Igor finished working on UTI generation task at IBQ, testing</li></ul>RegReporting - To be architecture draft is done - to enhance further - no resources this weekEDW<ul><li>Emir-Refit margin report functionality is testing - bugfixing</li><li>Anna DSB files upload in progress</li><li>FIRS data load is in progress</li><li>Test activities support required to fix Qort load</li><li>new SR (SFTR qustionnarie) is in development</li><li>to stop NSD services at UK</li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>Fixing bugs after versions upgrade & DB migrations</li><li>UK. FIRDS instruments export issue</li><li>EP. Upgrade Artemis to UK state</li></ul> | 
| top 3-5 points | 
| В понедельник ждем выход Жидкова на шину | 
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

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - доделали Trade Confirmation по продуктам. Тестируем загрузку сделок из QUIK через Exporter.</li><li>BCSGL - в TSL сделали донастройки для нового продукта Bank Deposit</li><li>BCSUK - собрали статистику ISIN-ов в рамках аудит запроса от CUSIP. Сделали мелкий багфиксинг по задачам Лены Баско.</li></ul>

IBQ: Продолжаем делать аналитику и разработку по проекту EMIR Refit. Сделали доработки по двум критичным SR по загрузке неторговый поручений и DVP / RVP сделок

CRM **EMIR REFIT:** 

<ul><li>Web form UI is finalized</li><li>Integrational Selects are changed to contain new fields</li><li>Test data added on sandbox</li></ul> **Service Cloud:** <ul><li>Recieving and analysing setup costs and technical options with current vendor and new CY resser of SF products.</li><li>Asking Salesforce directly for setup options with current CY org</li></ul> **Project K - ** Asked to add 10 MD to our evaluation since new requiments (QI status on CY) appeared **Finalizing current CRM developement pipeline**   **overview** Riskroom:<ul><li>SL3: had to fight with UK database problems consequences; also there was a request to get BBG prices for particular list of ISINs</li><li>ArmRm - meeting with Robert, all seems to be implemented, need feedback from production usage</li><li>qkCurrencyRate function replacement for UK - deployed, qkSecurities dependency eliminated, ready to switch off QUIK</li><li>REQ: CMA room enhancements for CDS portfolio calc for Emir/refit - UAT</li></ul>FX:<ul><li>Still having of time requests to database from ntpro2db - timeout enlarged, implemented to prod, to monitor</li><li>Banded tariffication - installed to prod, working on issues found</li><li>Unusual client activity alarm is at prod, also some minor changed deployed</li><li>DynRep: started to develop, no test data</li><li>News portal: minor changes, also to sort out some users do have some role</li></ul>OneTick, SFTR:<ul><li>OneTick: new release planned for Monday</li><li>Murex project: some minor activities, waiting for analysis</li><li>to plan new SR (qustionnarie) - analysis</li></ul>EMIR/REFIT:<ul><li>Oleg/Stas are working on the tasks</li><li>Igor finished working on UTI generation task at IBQ, testing</li></ul>RegReporting - To be architecture draft is done - to enhance further - no resources this weekEDW<ul><li>Emir-Refit margin report functionality is testing - bugfixing</li><li>Anna DSB files upload in progress</li><li>FIRS data load is in progress</li><li>Test activities support required to fix Qort load</li><li>new SR (SFTR qustionnarie) is in development</li><li>to stop NSD services at UK</li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>Fixing bugs after versions upgrade & DB migrations</li><li>UK. FIRDS instruments export issue</li><li>EP. Upgrade Artemis to UK state</li></ul> | 
| top 3-5 points | 
| В понедельник ждем выход Жидкова на шину | 







*****

[[category.storage-team]] 
[[category.confluence]] 
