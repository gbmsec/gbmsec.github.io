





| CHG

 | 
| Alexey Dorogov

 | 
|    

 | 
| Согласовали временное решение по отключению проверки на санкционность в Кондоре, получили задачу на реализацию этогоДелаем ревью серверов Корта и IBQIBQ:<ul><li>Работаем над текущими задачами в рамках SR и Bugs, а также по проектам AIX, TTCY и субброкерской схеме.</li></ul>EDW:<ul><li>SCS both version bloomberg file load</li><li>Fix mapping to upload securities type from BBG</li><li>Emir Portfolio testing</li></ul>ESB<ul><li>Migration to Kubernetes</li><li>ArgoCD for kubernetes deployments</li><li>SalesForce - Calypso event based integration</li><li>AIX integration</li></ul>RR<ul><li>Moving forward with CASS/TTCA projects (slower this week due to vacations).</li><li>Prepare moving to UK database cluster: hourly plan created.</li><li>Faced some unexplained behavior of services in k8s unexpectedly lost db connection.</li></ul>FX
1. Подготовка сервисов к переключению на кроссовое соединение
1. [FOIT-113](http://jira/browse/FOIT-113) - Вывели USD/CNH для Retail на прод
1. Запросили доступ к представления ИБСО для реализации реконсиляции сделок Retail
1.  **Emergency Rate**  - UAT алгоритма удаления экстремумов по bid и ask 
1. Консультации FX Desk по работе FIX протокола и разработке сервисов

Kondor
1. Принято решение об отмене проверки сделок на санкционность при загрузке их из ФО систем. Заведен SR.
1. При общении с FX деском принято решение провести ревизию используемого функционала.
1. Внеплановым релизом выведена доработка по поддержке sub-brokerage.
1. Согласовано с бизнесом к-во лицензий, которые они готовы у себя оставить.

 | 
| top 3-5 points | 
| Что делает DBA для Kondor Team 1. Он сопровождает кластер ag-lradiusdb, включая мониторинг его хелси. 2. Участвует в создании инстанса кластера для переезда наших бд экспортера на кластер ag-lradiusdb 3. Помогает в разборе проблем с перфомансом наших процедер на SQL серверах. 4. Переносит нам бд на тесте при переливке тестов с прода. 5. Поднимает нам резервные бд в случае утери данных. 6. Участвует со стороны дба в разборе инцидентов связанных с бд.Что делает DBA для RR Team 1. Интеграция в РР реализована с использование MS SQL очередей. DBA участвет в решении проблем с интеграцией, в случаях проблем с очередями 2. Решение проблем со снятием и восстановлением бэкапов, репликации на тесты, проблем с TempDB 3. Корректировка dba скриптов по снятию дампов и восстановлению с учетом текущих практик и требований | 
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
| Согласовали временное решение по отключению проверки на санкционность в Кондоре, получили задачу на реализацию этогоДелаем ревью серверов Корта и IBQIBQ:<ul><li>Работаем над текущими задачами в рамках SR и Bugs, а также по проектам AIX, TTCY и субброкерской схеме.</li></ul>EDW:<ul><li>SCS both version bloomberg file load</li><li>Fix mapping to upload securities type from BBG</li><li>Emir Portfolio testing</li></ul>ESB<ul><li>Migration to Kubernetes</li><li>ArgoCD for kubernetes deployments</li><li>SalesForce - Calypso event based integration</li><li>AIX integration</li></ul>RR<ul><li>Moving forward with CASS/TTCA projects (slower this week due to vacations).</li><li>Prepare moving to UK database cluster: hourly plan created.</li><li>Faced some unexplained behavior of services in k8s unexpectedly lost db connection.</li></ul>FX
1. Подготовка сервисов к переключению на кроссовое соединение
1. [FOIT-113](http://jira/browse/FOIT-113) - Вывели USD/CNH для Retail на прод
1. Запросили доступ к представления ИБСО для реализации реконсиляции сделок Retail
1.  **Emergency Rate**  - UAT алгоритма удаления экстремумов по bid и ask 
1. Консультации FX Desk по работе FIX протокола и разработке сервисов

Kondor
1. Принято решение об отмене проверки сделок на санкционность при загрузке их из ФО систем. Заведен SR.
1. При общении с FX деском принято решение провести ревизию используемого функционала.
1. Внеплановым релизом выведена доработка по поддержке sub-brokerage.
1. Согласовано с бизнесом к-во лицензий, которые они готовы у себя оставить.

 | 
| top 3-5 points | 
| Что делает DBA для Kondor Team 1. Он сопровождает кластер ag-lradiusdb, включая мониторинг его хелси. 2. Участвует в создании инстанса кластера для переезда наших бд экспортера на кластер ag-lradiusdb 3. Помогает в разборе проблем с перфомансом наших процедер на SQL серверах. 4. Переносит нам бд на тесте при переливке тестов с прода. 5. Поднимает нам резервные бд в случае утери данных. 6. Участвует со стороны дба в разборе инцидентов связанных с бд.Что делает DBA для RR Team 1. Интеграция в РР реализована с использование MS SQL очередей. DBA участвет в решении проблем с интеграцией, в случаях проблем с очередями 2. Решение проблем со снятием и восстановлением бэкапов, репликации на тесты, проблем с TempDB 3. Корректировка dba скриптов по снятию дампов и восстановлению с учетом текущих практик и требований | 







*****

[[category.storage-team]] 
[[category.confluence]] 
