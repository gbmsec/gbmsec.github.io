





| CHG

 | 
| Alexey Dorogov

 | 
| 

 | 
| ESB

<ul><li>ESB Segregation: RabbitMQ</li><li>KondorUK decomission tasks</li><li>Calypso nonUK integrations</li></ul>

Riskroom:

<ul><li>Datastructure around counterparties/groups reworked upun users feedback</li><li>Got more clarifications on Limits calculation reqs</li></ul>FX:

<ul><li>Weekend delayed trades: fix delivered</li><li>FINAM report: got data on netting via ESB mail</li><li>Started to work on Emergency dashboard bug and UI enhancement</li></ul>OneTick:

<ul><li>working on several SDs from support to sort out monitoring issues</li></ul>

Calypso:

<ul><li>Занимаемся задачей по переходу с FIX сообщений на загрузку из QUIK экспортера. На этой неделе согласовали, что шина будет делать преобразование к FIX подобному формату.</li><li>Calypso Non UK - настроили интеграцию с Bloomberg (пока без шифрования). Настроили подключения в тесте Calypso PREP Non UK к шине Non UK. DBA настроили развертывание в Calypso PROD Non UK ежедневное обновление из безтранзакционного дампа UK + скрипты по очистке статики UK.</li><li>Декомиссия Kondor+ в периметре UK - в релиз выходят задачи по распараллеливанию сделок QUIK OMS / TOMS в Calypso UK и Kondor+. Передача сделок из Kondor+ в Calypso отключается. Перенастроена реконселяция между Kondor и Calypso, чтобы сверять по параметрам (без привязки к кондоровому идентификатору).</li><li>Провели планирование задач на следующий спринт</li></ul>IBQ:

<ul><li>Делаем аналитику по проекту EMIR Refit.</li><li>Сделали задачи по сетапу FAB в периметре Кипра.</li></ul>Kondor
1. На эти выходные планируется старт первого этапа отключения К+ в UK - parallel run. Отключаем связи К+ с Калипсо по UK.
1. Атриум - получили от безопасности требования по удаленному доступу, передали Систематике.
1. Презентовали новое решение по ТОМС.
1. В процессе чистка фондирующих позиций. Взят в анализ вопрос о функционале, который мы также еще можем отключить.
1. В этом релизе выводится задачу по сверке класс-кодов в Quik, определенных для нашего экспортера и настроенных для загрузки у нас. 

 | 
| top 3-5 points | 
| 1) FX. Нашли, что на стороне сервисов FX используется на фронте платный плагин. Мы его не закупали. Сейчас предполагаем, что в нем есть баг. Оплатить подписку не можем, т.к. они не продают русским.По ФХ в очередной раз активизация и есть задачи. А это значит меньше времени на другую разработку.2) !!! Совсем нет прогресса по  поиску. Мы так вообще никого не найдем. Я не понимаю кто и что может с этом сделать | 
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
| ESB

<ul><li>ESB Segregation: RabbitMQ</li><li>KondorUK decomission tasks</li><li>Calypso nonUK integrations</li></ul>

Riskroom:

<ul><li>Datastructure around counterparties/groups reworked upun users feedback</li><li>Got more clarifications on Limits calculation reqs</li></ul>FX:

<ul><li>Weekend delayed trades: fix delivered</li><li>FINAM report: got data on netting via ESB mail</li><li>Started to work on Emergency dashboard bug and UI enhancement</li></ul>OneTick:

<ul><li>working on several SDs from support to sort out monitoring issues</li></ul>

Calypso:

<ul><li>Занимаемся задачей по переходу с FIX сообщений на загрузку из QUIK экспортера. На этой неделе согласовали, что шина будет делать преобразование к FIX подобному формату.</li><li>Calypso Non UK - настроили интеграцию с Bloomberg (пока без шифрования). Настроили подключения в тесте Calypso PREP Non UK к шине Non UK. DBA настроили развертывание в Calypso PROD Non UK ежедневное обновление из безтранзакционного дампа UK + скрипты по очистке статики UK.</li><li>Декомиссия Kondor+ в периметре UK - в релиз выходят задачи по распараллеливанию сделок QUIK OMS / TOMS в Calypso UK и Kondor+. Передача сделок из Kondor+ в Calypso отключается. Перенастроена реконселяция между Kondor и Calypso, чтобы сверять по параметрам (без привязки к кондоровому идентификатору).</li><li>Провели планирование задач на следующий спринт</li></ul>IBQ:

<ul><li>Делаем аналитику по проекту EMIR Refit.</li><li>Сделали задачи по сетапу FAB в периметре Кипра.</li></ul>Kondor
1. На эти выходные планируется старт первого этапа отключения К+ в UK - parallel run. Отключаем связи К+ с Калипсо по UK.
1. Атриум - получили от безопасности требования по удаленному доступу, передали Систематике.
1. Презентовали новое решение по ТОМС.
1. В процессе чистка фондирующих позиций. Взят в анализ вопрос о функционале, который мы также еще можем отключить.
1. В этом релизе выводится задачу по сверке класс-кодов в Quik, определенных для нашего экспортера и настроенных для загрузки у нас. 

 | 
| top 3-5 points | 
| 1) FX. Нашли, что на стороне сервисов FX используется на фронте платный плагин. Мы его не закупали. Сейчас предполагаем, что в нем есть баг. Оплатить подписку не можем, т.к. они не продают русским.По ФХ в очередной раз активизация и есть задачи. А это значит меньше времени на другую разработку.2) !!! Совсем нет прогресса по  поиску. Мы так вообще никого не найдем. Я не понимаю кто и что может с этом сделать | 







*****

[[category.storage-team]] 
[[category.confluence]] 
