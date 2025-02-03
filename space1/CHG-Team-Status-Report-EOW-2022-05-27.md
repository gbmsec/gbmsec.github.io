





| CHG

 | 
| Alexey Dorogov

 | 
|    

 | 
| Kondor
1. Выделение репортинга odd-lot в отдельный поток на общей встрече команды решено отложить до лучших времен.
1. Наконец-то пришла информация о новых сроков переноса функционала по полному обслуживанию "родных" займов Казны в КХД - июнь.
1. По замечаниям пред-архитектурного комитета доработана функциональная схема. По замечаниям Вити отработано не полностью, поскольку я не получил ответы на свои вопросы.
1. Как emergency change выведено исправление по загрузке исполнений из Корт
1. Также в приоритетном порядке ведутся работы по проекту  [PRJ-271](http://jira/browse/PRJ-271)- jiraissues.unexpected.error Jira issues is not available  (Sub-Brokerage operational scheme)

Calypso<ul><li>Продолжаем заниматься приоритетными задачами по проекту FAB и CASS. </li></ul>ESB<ul><li>ESB Migration to Kubernetes. Reports</li><li>SB Migration to Kubernetes. Fix-adapter properties</li><li>ESB Migration to Kubernetes. BAM&Grafana routes</li></ul>EDW<ul><li>Technical debt</li><li>EMIR reconciliation</li><li>Reporting Analitics</li></ul>CPORT Готов дисклеймер для ресерчCRM1) Calypso full scale integration - предоставлены тестовые данные для интеграции, а также тестовый csv для реконcеляции  2) LEI Expiry autoupdate - подготовлены и залиты в систему исторические данные. LEI истёк для нескольких десятков клиентов в статусе Live, CRM проверяют этот список, после чего будут включены уведомления для Compliance/CRM на постоянной основе 3) User turn down improved process - разрабатываем специальную страницу для ускорения и лучшего контроля процесса отключения пользователя. Всё реализовано на одной специализированной странице: shortcut-ы отчетов для переноса связанных с пользователем данных в системе, выведение списком всех процессов согласования с участием пользователя + инструкция по отключению 4) Conga Courier rebuild with Conga Composer+Batch - отключился вендорский продукт доставки отчетов (расширение Salesforce), функционал переносится на заменяющее решение Conga Composer+BatchRRSuccessfully deployed intraday limits files generation from service to file storage (for Succession and Moex). Implemented separation of static fields for 5-times a day requests to BBG, which should reduce overall cost. | 
|  | 
| 1) Переговорил с Коноваловой по поводу снижения SLA и времени поддержки. Успеха нет. ОПС планирует работу с 8 до 21. У нас не будет ресурсво на такую поддержку. Не понятно как мы достигнем снижения SLA и самое главное времени поддержки. 2) Утренней сессии не будет для Prime, что может чуть облегчить жизнь, но по факту совсем не сильно3)  **!!!**  Нужно сообщить Никите как и когда мы сможем ему вернуть 54 EUR за посылку | 
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
| Kondor
1. Выделение репортинга odd-lot в отдельный поток на общей встрече команды решено отложить до лучших времен.
1. Наконец-то пришла информация о новых сроков переноса функционала по полному обслуживанию "родных" займов Казны в КХД - июнь.
1. По замечаниям пред-архитектурного комитета доработана функциональная схема. По замечаниям Вити отработано не полностью, поскольку я не получил ответы на свои вопросы.
1. Как emergency change выведено исправление по загрузке исполнений из Корт
1. Также в приоритетном порядке ведутся работы по проекту  [PRJ-271](http://jira/browse/PRJ-271)- jiraissues.unexpected.error Jira issues is not available  (Sub-Brokerage operational scheme)

Calypso<ul><li>Продолжаем заниматься приоритетными задачами по проекту FAB и CASS. </li></ul>ESB<ul><li>ESB Migration to Kubernetes. Reports</li><li>SB Migration to Kubernetes. Fix-adapter properties</li><li>ESB Migration to Kubernetes. BAM&Grafana routes</li></ul>EDW<ul><li>Technical debt</li><li>EMIR reconciliation</li><li>Reporting Analitics</li></ul>CPORT Готов дисклеймер для ресерчCRM1) Calypso full scale integration - предоставлены тестовые данные для интеграции, а также тестовый csv для реконcеляции  2) LEI Expiry autoupdate - подготовлены и залиты в систему исторические данные. LEI истёк для нескольких десятков клиентов в статусе Live, CRM проверяют этот список, после чего будут включены уведомления для Compliance/CRM на постоянной основе 3) User turn down improved process - разрабатываем специальную страницу для ускорения и лучшего контроля процесса отключения пользователя. Всё реализовано на одной специализированной странице: shortcut-ы отчетов для переноса связанных с пользователем данных в системе, выведение списком всех процессов согласования с участием пользователя + инструкция по отключению 4) Conga Courier rebuild with Conga Composer+Batch - отключился вендорский продукт доставки отчетов (расширение Salesforce), функционал переносится на заменяющее решение Conga Composer+BatchRRSuccessfully deployed intraday limits files generation from service to file storage (for Succession and Moex). Implemented separation of static fields for 5-times a day requests to BBG, which should reduce overall cost. | 
|  | 
| 1) Переговорил с Коноваловой по поводу снижения SLA и времени поддержки. Успеха нет. ОПС планирует работу с 8 до 21. У нас не будет ресурсво на такую поддержку. Не понятно как мы достигнем снижения SLA и самое главное времени поддержки. 2) Утренней сессии не будет для Prime, что может чуть облегчить жизнь, но по факту совсем не сильно3)  **!!!**  Нужно сообщить Никите как и когда мы сможем ему вернуть 54 EUR за посылку | 







*****

[[category.storage-team]] 
[[category.confluence]] 
