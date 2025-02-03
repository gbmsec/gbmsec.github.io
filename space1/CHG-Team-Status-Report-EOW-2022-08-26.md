





| CHG

 | 
| Alexey Dorogov

 | 
|    

 | 
| По SS - нашел много пользователей, кто не заблокирован в программе. Отправил на блокировкуПровел звонок в IBQ и Колей Дружининым. Наметили план, чтобы он начал по задачам сервисов работать. Посмотрим что получится...RRMore preparations and test to move to UK database cluster. ESB<ul><li>Migration to Kubernetes</li><li>SalesForce - Calypso event based integration</li><li>AIX integration</li><li>SalesForce - TAINA integration</li></ul>EDW<ul><li>SCS. Intraday sanction lists generation</li><li>Report / reconciliation of the data in EDW with the data sent to SFTR</li><li>EMIR Portfolio Schedule Generation, EMIR Portfolio GUI , EMIR Portfolio - Export and Save files

</li></ul>IBQ<ul><li>Доделали все задачи по проекту AIX (появились новые от ОПС, не заакцептованные на Проектном комитете, их пока не делаем)</li><li>Доделали все задачи по проекту субброкерской схемы</li></ul>Kondor
1. В компании больше не работает Рохлина (вела проект по переносу фондирования в КХД).
1. Принято решение по шарингу ресурса Коли с командой EDW в задачах разработки на C#. Буду определять процентовку участия при планировании спринтов. Согласовали время проведения утренних ежедневных встреч команд для участия Коли и там, и сям.
1. Выполнили разработку по отмене проверки санкций на сделках, приходящих из ФО систем.
1. Собран и упорядочен список неописанного функционала. По мере свободных ресурсов будем описывать.
1. Отключение ненужных позиций Equity - на релизной встрече вспомнили, что забыли про РР. Выведено из этого релиза.

FX
1. Перевести пилотные сервисы на кроссовое подключени - переносится на следующую неделю, ждем возвращения из отпуска Данилы
1. Протестировали вывод шины из процесса передачи котировок в Менялке, ждем согласования от Владимира на вывод в прод
1. Добавили новую валютную пару USD/CNY в сервис котирования для корпоративных клиентов.
1. Консультации FX Desk по работе FIX протокола и разработке сервисов

CRM **1) LEI Code auto-notice: SELECT filter fix** FIxing logic so that we start checking client LEI 10 days before expiry. This way we stay updated and do not issue any extensive notifiations. **2) Risk Questionnaire attachements upload fix** We generally upload risk parameters and attachements via web forms now. For this web form we missed some scenarios for attachement in the connector logic. So we had to manually tranfer missing data and improve the connect to work for all web form responses. **3) New US_parent parameter for UMR ANNA** Group requested from us that we store a paramater for the cases when Client/CP has a parent that is US originated. This is required for some calculations to meet UMR. The agreement is that this parameter will appear whenever there is an ISDA agreement and marked "yes" when US originated parent exists. **4) CRM mass mailings** Another UAT and fixes iteration was made and final version is to appear in the next release. **5) "Cancel case" data reverse fix ** When onboarding case is cancelled some of the process data is reversed to previous values. Found and fixed errors appearing in some scenarious of reversion the data. | 
|  | 
| !!! Задай вопрос на встрече в понедельник - кто будет делать коммуникацию на трейдеров, что теперь они работают без проверки на Санкции в Кондоре. Это было в Action points договоренность отключения санкций в К+. Но я не видел коммуникацию на трейдаков. 

![](images/storage/image2022-8-26_18-32-12.png)

 | 
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
| По SS - нашел много пользователей, кто не заблокирован в программе. Отправил на блокировкуПровел звонок в IBQ и Колей Дружининым. Наметили план, чтобы он начал по задачам сервисов работать. Посмотрим что получится...RRMore preparations and test to move to UK database cluster. ESB<ul><li>Migration to Kubernetes</li><li>SalesForce - Calypso event based integration</li><li>AIX integration</li><li>SalesForce - TAINA integration</li></ul>EDW<ul><li>SCS. Intraday sanction lists generation</li><li>Report / reconciliation of the data in EDW with the data sent to SFTR</li><li>EMIR Portfolio Schedule Generation, EMIR Portfolio GUI , EMIR Portfolio - Export and Save files

</li></ul>IBQ<ul><li>Доделали все задачи по проекту AIX (появились новые от ОПС, не заакцептованные на Проектном комитете, их пока не делаем)</li><li>Доделали все задачи по проекту субброкерской схемы</li></ul>Kondor
1. В компании больше не работает Рохлина (вела проект по переносу фондирования в КХД).
1. Принято решение по шарингу ресурса Коли с командой EDW в задачах разработки на C#. Буду определять процентовку участия при планировании спринтов. Согласовали время проведения утренних ежедневных встреч команд для участия Коли и там, и сям.
1. Выполнили разработку по отмене проверки санкций на сделках, приходящих из ФО систем.
1. Собран и упорядочен список неописанного функционала. По мере свободных ресурсов будем описывать.
1. Отключение ненужных позиций Equity - на релизной встрече вспомнили, что забыли про РР. Выведено из этого релиза.

FX
1. Перевести пилотные сервисы на кроссовое подключени - переносится на следующую неделю, ждем возвращения из отпуска Данилы
1. Протестировали вывод шины из процесса передачи котировок в Менялке, ждем согласования от Владимира на вывод в прод
1. Добавили новую валютную пару USD/CNY в сервис котирования для корпоративных клиентов.
1. Консультации FX Desk по работе FIX протокола и разработке сервисов

CRM **1) LEI Code auto-notice: SELECT filter fix** FIxing logic so that we start checking client LEI 10 days before expiry. This way we stay updated and do not issue any extensive notifiations. **2) Risk Questionnaire attachements upload fix** We generally upload risk parameters and attachements via web forms now. For this web form we missed some scenarios for attachement in the connector logic. So we had to manually tranfer missing data and improve the connect to work for all web form responses. **3) New US_parent parameter for UMR ANNA** Group requested from us that we store a paramater for the cases when Client/CP has a parent that is US originated. This is required for some calculations to meet UMR. The agreement is that this parameter will appear whenever there is an ISDA agreement and marked "yes" when US originated parent exists. **4) CRM mass mailings** Another UAT and fixes iteration was made and final version is to appear in the next release. **5) "Cancel case" data reverse fix ** When onboarding case is cancelled some of the process data is reversed to previous values. Found and fixed errors appearing in some scenarious of reversion the data. | 
|  | 
| !!! Задай вопрос на встрече в понедельник - кто будет делать коммуникацию на трейдеров, что теперь они работают без проверки на Санкции в Кондоре. Это было в Action points договоренность отключения санкций в К+. Но я не видел коммуникацию на трейдаков. 

![](images/storage/image2022-8-26_18-32-12.png)

 | 







*****

[[category.storage-team]] 
[[category.confluence]] 
