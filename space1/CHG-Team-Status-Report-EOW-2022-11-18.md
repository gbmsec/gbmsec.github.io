





| CHG

 | 
| 

 | 
|    

 | 
| <ul><li>решаем проблему с Гращенко</li><li>уходит А. Мошков. Нужно согласовать добавки для Тимешова и Сорокина</li><li>нужно не потерять К. Дружинина и согласовать изменение ЗП</li></ul>

EDW

<ul><li>New trade CA uploadtng</li><li>SCS. Change filter logic for RUDATA</li><li>Entity split. Create script to data uploading</li><li>EMIR portfolio</li></ul>

Calypso:

<ul><li>Протестировали задачу по миграции MiFID с Capitech на Unavista. Планируем вывести ее в релиз.</li><li>Продолжается тестирование новой версии Calypso 16.22.7.3, работаем над ошибками связанными с Bloomberg. На текущий момент успешно пройдено 90% из тестов Вадима.</li><li>По CASS провели демо по FX OTC сделкам. Продолжаем заниматься исправлением ошибок, которые находятся в рамках UAT тестирования.</li><li>В рамках задачи CLPS-6756 готовим XML с миграционными сделками для выравнивания позиций для команды CA в Inventory. Тестируем их в PREP перед будущим выкатом в PROD. Провели демонстрацию заведения этих сделок команде саппорта.</li><li>Продолжается выверка данных между SalesForce и Calypso в рамках тестирования интеграции.</li></ul>IBQ:

<ul><li>Работаем над текущими задачами. Багфиксинг и небольшие SR</li><li>Провели планирование задач нового спринта.</li><li> Вывод релиза в PROD.</li><li>Продолжаем шарить экспертизу по сопровождению QORT и сопутствующих сервисов внутри QORT Support и командой Оли Медведевой. А также предоставлять доступ в QORT и сопутствующие сервисы.</li><li>По тестовым средам QORT, мы хотим восстановить свежую базу, чтобы на свежих данных можно было проверить рекомендации от ARQA по тем обращениям, что у нас есть в работе.</li><li>Пытаемся навести порядок в картах Euroclear CY и UK, а также определить у кого есть карты Администратора. По уволенным сотрудникам планируется запустить процедуру блокировки карт.</li></ul>RRCASS: first pass thru test of excess calculation on Calypso so data, sending transfers to Calypso and getting ACK is doneFX: testing by BA of interest calculation functionalitySL3: prop vop calculation performance increased with fixing an old bugUK/non UK: market data as is Various: <ul><li>Succession limits generation is stopped, also in intraday</li><li>Preparing to switch off UK2 exporter</li></ul>Refactoring:<ul><li>limits generation engine to store generated data to reuse</li><li>integration from ms sql to rabbitMq</li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>Migration to Kubernetes</li><li>K8S containers tuning</li></ul> | 
| top 3-5 points | 
| В рамках обсуждений проекта Prime Segregation все больше получаю обратную связь, которую нуэно проинформировать. Владельцы многих процессов считают, что к ним должны прийти и организовать их изменения на их стороне по процессам. Моя позиция другая - владельцы процессов имеют информацию по отделению Прайма и сами должны организовать и спланировать изменения, которые им необходимы. Тут нужно как то синхронизоваться, т.к. я не планировал и меня не хватит бегать за всеми. И я считаю, что не правильно решать проблемы в процессах других подразделений | 
|  --- | 
|  --- | 
|  --- | 
|  --- | 
|  --- | 
|  --- | 
| CHG

 | 
| 

 | 
|    

 | 
| <ul><li>решаем проблему с Гращенко</li><li>уходит А. Мошков. Нужно согласовать добавки для Тимешова и Сорокина</li><li>нужно не потерять К. Дружинина и согласовать изменение ЗП</li></ul>

EDW

<ul><li>New trade CA uploadtng</li><li>SCS. Change filter logic for RUDATA</li><li>Entity split. Create script to data uploading</li><li>EMIR portfolio</li></ul>

Calypso:

<ul><li>Протестировали задачу по миграции MiFID с Capitech на Unavista. Планируем вывести ее в релиз.</li><li>Продолжается тестирование новой версии Calypso 16.22.7.3, работаем над ошибками связанными с Bloomberg. На текущий момент успешно пройдено 90% из тестов Вадима.</li><li>По CASS провели демо по FX OTC сделкам. Продолжаем заниматься исправлением ошибок, которые находятся в рамках UAT тестирования.</li><li>В рамках задачи CLPS-6756 готовим XML с миграционными сделками для выравнивания позиций для команды CA в Inventory. Тестируем их в PREP перед будущим выкатом в PROD. Провели демонстрацию заведения этих сделок команде саппорта.</li><li>Продолжается выверка данных между SalesForce и Calypso в рамках тестирования интеграции.</li></ul>IBQ:

<ul><li>Работаем над текущими задачами. Багфиксинг и небольшие SR</li><li>Провели планирование задач нового спринта.</li><li> Вывод релиза в PROD.</li><li>Продолжаем шарить экспертизу по сопровождению QORT и сопутствующих сервисов внутри QORT Support и командой Оли Медведевой. А также предоставлять доступ в QORT и сопутствующие сервисы.</li><li>По тестовым средам QORT, мы хотим восстановить свежую базу, чтобы на свежих данных можно было проверить рекомендации от ARQA по тем обращениям, что у нас есть в работе.</li><li>Пытаемся навести порядок в картах Euroclear CY и UK, а также определить у кого есть карты Администратора. По уволенным сотрудникам планируется запустить процедуру блокировки карт.</li></ul>RRCASS: first pass thru test of excess calculation on Calypso so data, sending transfers to Calypso and getting ACK is doneFX: testing by BA of interest calculation functionalitySL3: prop vop calculation performance increased with fixing an old bugUK/non UK: market data as is Various: <ul><li>Succession limits generation is stopped, also in intraday</li><li>Preparing to switch off UK2 exporter</li></ul>Refactoring:<ul><li>limits generation engine to store generated data to reuse</li><li>integration from ms sql to rabbitMq</li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>Migration to Kubernetes</li><li>K8S containers tuning</li></ul> | 
| top 3-5 points | 
| В рамках обсуждений проекта Prime Segregation все больше получаю обратную связь, которую нуэно проинформировать. Владельцы многих процессов считают, что к ним должны прийти и организовать их изменения на их стороне по процессам. Моя позиция другая - владельцы процессов имеют информацию по отделению Прайма и сами должны организовать и спланировать изменения, которые им необходимы. Тут нужно как то синхронизоваться, т.к. я не планировал и меня не хватит бегать за всеми. И я считаю, что не правильно решать проблемы в процессах других подразделений | 







*****

[[category.storage-team]] 
[[category.confluence]] 
