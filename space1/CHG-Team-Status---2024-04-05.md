





| CHG

 | 
| Alexey 

 | 
| 

 | 
| Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - согласовали концепцию букирования CFD сделок. В работе сетап агентский схемы для РЕПО. Аналитика и постановка задач на доработку по FATCA, CRS. Тестирование отчетности по MiFID. Отдали в UAT на тестирование начисление комиссий по клиентам. Делаем мелкие правки по CDS-ам.</li><li>BCSGL - багфиксинг по TSL. Вместе с пользователями тестируем разделение прав к данным по PO.</li><li>BCSUK - настроили реализацию PnL по FI продуктам в рамках бага.</li></ul>IBQ:

<ul><li>Активно тестируем сделанные задачи по проекту EMIR Refit. Идет UAT + багфиксинг.</li></ul>Riskroom:<ul><li>continue to analyze tasks related to decommission of Qort</li><li>switched off some jobs not used at UK</li><li>new task "Limits to MM" was initially discussed, waiting for SR and reqs - still in progress</li><li>to plan task of moving Quik autolimits functionality to EP</li><li>ARM RM limits are loaded from the file provided</li></ul>FX:<ul><li>discussions on results of Q1 and plans for Q2</li><li>Unusual client activity alarm is at prod, more task to show it at UI - UAT deployed after tech review</li><li>DynRep: stopping development until stable prod-like env for testing</li><li>Task to analyze productivity of Unusual activities monitor</li></ul>OneTick, SFTR:<ul><li>OneTick: implementation for marex - UAT, new reqs arrives, waiting</li><li>to plan new SR (qustionnarie) - analysis - still question if any changes needed - dev started on that (Stas)</li></ul>EMIR/REFIT:<ul><li>UTI generation task at IBQ is testing</li><li>Anna DSB data load service at UAT</li><li>FIRDS loader to EDW service at UAT, need code review</li><li>RegReporting</li></ul><ul><li>Discussions on reprting service approach</li></ul>EDW<ul><li>Emir-Refit margin report functionality is testing - bugfixing</li><li>Test activities support required to fix Qort load</li><li>new SR (SFTR qustionnarie) development is done, testing</li><li>to stop NSD services at UK (not done)</li></ul>Kondor
1. Новый разработчик выходит 11.04. Надеюсь, что как минимум с июня будет уже приносить пользу, до этого как-то будем вливать в процесс и обучать.
1. Полностью подготовлена инфраструктура под Атриум.
1. От бизнеса приходят "срочные" задачи (что вне проекта Атриум): загрузка и учет дат офферт облигаций, Product Governance. Ресурсов на них нет.  **Непонятно, как и с кем согласовывать снятие ресурсов с проекта перехода на Атриум на срочные задачи других направлений - что повлечет за собой сдвиг сроков проекта Атриум.** 
1. Для тестирования передачи сделок ОТС Кипр ИБ из Атриум в Корт подготовлен тестовый комплекс.
1. Проведена встреча с инфра по организации DR Атриума.

 | 
| top 3-5 points | 
| 1) Решить вопрос по бюджету Калипсо на 24 год по части нон-ЮК. Катя писала. Что делаем ?2) Оч медленно движутся дела по оплате счетов, согласованию договоров. Все на ручнике и кучу внимания надо.3) Договор в ВДКом на апрель еще не подписан и не согласован4) ВДКом - работы за февраль еще не оплачены5) Прислали оценку по веб-кабинету на Кипр. Надо определить потребность в ставках на нашей стороне **!!! From Kostya** <ul><li>need R/W access to Oracle EDW_PROD in UK to solve urgent SL3 cases</li><li>still more reqs for IBQ-6142 (Marex), cannot finish development for this task declared as urgent in OneTick service</li></ul> **!!! Kondor**  **Непонятно, как и с кем согласовывать снятие ресурсов с проекта перехода на Атриум на срочные задачи других направлений - что повлечет за собой сдвиг сроков проекта Атриум. **  | 
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

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - согласовали концепцию букирования CFD сделок. В работе сетап агентский схемы для РЕПО. Аналитика и постановка задач на доработку по FATCA, CRS. Тестирование отчетности по MiFID. Отдали в UAT на тестирование начисление комиссий по клиентам. Делаем мелкие правки по CDS-ам.</li><li>BCSGL - багфиксинг по TSL. Вместе с пользователями тестируем разделение прав к данным по PO.</li><li>BCSUK - настроили реализацию PnL по FI продуктам в рамках бага.</li></ul>IBQ:

<ul><li>Активно тестируем сделанные задачи по проекту EMIR Refit. Идет UAT + багфиксинг.</li></ul>Riskroom:<ul><li>continue to analyze tasks related to decommission of Qort</li><li>switched off some jobs not used at UK</li><li>new task "Limits to MM" was initially discussed, waiting for SR and reqs - still in progress</li><li>to plan task of moving Quik autolimits functionality to EP</li><li>ARM RM limits are loaded from the file provided</li></ul>FX:<ul><li>discussions on results of Q1 and plans for Q2</li><li>Unusual client activity alarm is at prod, more task to show it at UI - UAT deployed after tech review</li><li>DynRep: stopping development until stable prod-like env for testing</li><li>Task to analyze productivity of Unusual activities monitor</li></ul>OneTick, SFTR:<ul><li>OneTick: implementation for marex - UAT, new reqs arrives, waiting</li><li>to plan new SR (qustionnarie) - analysis - still question if any changes needed - dev started on that (Stas)</li></ul>EMIR/REFIT:<ul><li>UTI generation task at IBQ is testing</li><li>Anna DSB data load service at UAT</li><li>FIRDS loader to EDW service at UAT, need code review</li><li>RegReporting</li></ul><ul><li>Discussions on reprting service approach</li></ul>EDW<ul><li>Emir-Refit margin report functionality is testing - bugfixing</li><li>Test activities support required to fix Qort load</li><li>new SR (SFTR qustionnarie) development is done, testing</li><li>to stop NSD services at UK (not done)</li></ul>Kondor
1. Новый разработчик выходит 11.04. Надеюсь, что как минимум с июня будет уже приносить пользу, до этого как-то будем вливать в процесс и обучать.
1. Полностью подготовлена инфраструктура под Атриум.
1. От бизнеса приходят "срочные" задачи (что вне проекта Атриум): загрузка и учет дат офферт облигаций, Product Governance. Ресурсов на них нет.  **Непонятно, как и с кем согласовывать снятие ресурсов с проекта перехода на Атриум на срочные задачи других направлений - что повлечет за собой сдвиг сроков проекта Атриум.** 
1. Для тестирования передачи сделок ОТС Кипр ИБ из Атриум в Корт подготовлен тестовый комплекс.
1. Проведена встреча с инфра по организации DR Атриума.

 | 
| top 3-5 points | 
| 1) Решить вопрос по бюджету Калипсо на 24 год по части нон-ЮК. Катя писала. Что делаем ?2) Оч медленно движутся дела по оплате счетов, согласованию договоров. Все на ручнике и кучу внимания надо.3) Договор в ВДКом на апрель еще не подписан и не согласован4) ВДКом - работы за февраль еще не оплачены5) Прислали оценку по веб-кабинету на Кипр. Надо определить потребность в ставках на нашей стороне **!!! From Kostya** <ul><li>need R/W access to Oracle EDW_PROD in UK to solve urgent SL3 cases</li><li>still more reqs for IBQ-6142 (Marex), cannot finish development for this task declared as urgent in OneTick service</li></ul> **!!! Kondor**  **Непонятно, как и с кем согласовывать снятие ресурсов с проекта перехода на Атриум на срочные задачи других направлений - что повлечет за собой сдвиг сроков проекта Атриум. **  | 







*****

[[category.storage-team]] 
[[category.confluence]] 
