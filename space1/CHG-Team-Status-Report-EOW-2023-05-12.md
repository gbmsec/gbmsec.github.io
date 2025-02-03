





| CHG

 | 
| Alexey Dorogov

 | 
| 

 | 
| Kondor1. Проверили договоры Finastra. Вроде для разрыва отношений с января 2025 никаких действий принимать не надо - но на всякий случай послали запрос.2. Обновили версию Модулляра в тесте 2.3. Проработана архитектура ведения счетов и сделок по Казахстану. Послано на согласование DS.4. Пришли SR-ы на загрузку сделок из VCON.5. Провели ограничение прав на счета Кипра согласно запросу compliance. Остался вопрос по правам Казначейства - на стороне compliance.Calypso<ul><li>По CASS проекту - восстановили статику после обновления тестовой среды. По CMAR отчету планируем вывести в релиз предварительную версию отчета. </li><li>MiFID Post Trade Reporting - восстановили настройки после обновления теста и продолжаем тестирование функционала.</li><li>По проекту сетапа BCSKZ в Calypso UK  - восстановили статику после обновления тестовых сред. Ждем первую тестовую сделку из Кондора.</li></ul>IBQ:

<ul><li>Поддерживали тестирование новых инстансов QORT / IBQ на серверах Кипра.</li><li>Предоставили данные по запросу CySEC относительно MiFID II Transaction Report.</li><li>Планируем миграцию на новые сервера Кипра  </li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>ESB Segregation: Migration to Kubernetes - NonUK</li><li>ESB Segregation: Split EDW integrations</li><li>ClientPortal decomission</li></ul>RR<ul><li>Key users installed and can run RiskRoom EP </li><li>Some flows which is yet missing from ESB are duplicating via dblink from UK</li><li>Jobs review is done at PROD EP</li><li>BBG connectivity is checked via CY, all is fine </li><li>Reports schedules are not working, DBA task created</li></ul> | 
| top 3-5 points | 
| 1) AIX Morningсегодня оказался на чудной встрече - коллеги что то собрались тестирвоать по теме AIX Morning. мы долго готовили наше предложение, но в итоге услышали, что был НПС, на нем был ты и все вопросы по ИТ части к тебе.Я не знаю ничего что было согласовано, так же как и коллеги и с каким сетапом мы в итоге идем.Так нельзя делать проекты, информации ноль кто чего согласовал, какие проекты открыты и кто их ведет. Вообще информации ноль!от Миши Б:
1. SR по сверке ОМС UK против Калипсо так пока и не заведен, несмотря на то, что Наташей Рахмановой отсутствие данной  сверки было заявлено как show-stopper для отключения прогрузки сделок UK в К+.
1. Перевод фондирования в КХД и отказ от фондирования UK - нет ответа по статусу этих вопросов.
1. Статус определения системы для Казны (предложенное решение - Атриум) - не известен.

От Кости Е.<ul><li>BBG CY certificate is about to expire, KHD team informed</li><li>No possibility yet to setup Grafana minitoring at EP</li></ul> | 
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
| Kondor1. Проверили договоры Finastra. Вроде для разрыва отношений с января 2025 никаких действий принимать не надо - но на всякий случай послали запрос.2. Обновили версию Модулляра в тесте 2.3. Проработана архитектура ведения счетов и сделок по Казахстану. Послано на согласование DS.4. Пришли SR-ы на загрузку сделок из VCON.5. Провели ограничение прав на счета Кипра согласно запросу compliance. Остался вопрос по правам Казначейства - на стороне compliance.Calypso<ul><li>По CASS проекту - восстановили статику после обновления тестовой среды. По CMAR отчету планируем вывести в релиз предварительную версию отчета. </li><li>MiFID Post Trade Reporting - восстановили настройки после обновления теста и продолжаем тестирование функционала.</li><li>По проекту сетапа BCSKZ в Calypso UK  - восстановили статику после обновления тестовых сред. Ждем первую тестовую сделку из Кондора.</li></ul>IBQ:

<ul><li>Поддерживали тестирование новых инстансов QORT / IBQ на серверах Кипра.</li><li>Предоставили данные по запросу CySEC относительно MiFID II Transaction Report.</li><li>Планируем миграцию на новые сервера Кипра  </li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>ESB Segregation: Migration to Kubernetes - NonUK</li><li>ESB Segregation: Split EDW integrations</li><li>ClientPortal decomission</li></ul>RR<ul><li>Key users installed and can run RiskRoom EP </li><li>Some flows which is yet missing from ESB are duplicating via dblink from UK</li><li>Jobs review is done at PROD EP</li><li>BBG connectivity is checked via CY, all is fine </li><li>Reports schedules are not working, DBA task created</li></ul> | 
| top 3-5 points | 
| 1) AIX Morningсегодня оказался на чудной встрече - коллеги что то собрались тестирвоать по теме AIX Morning. мы долго готовили наше предложение, но в итоге услышали, что был НПС, на нем был ты и все вопросы по ИТ части к тебе.Я не знаю ничего что было согласовано, так же как и коллеги и с каким сетапом мы в итоге идем.Так нельзя делать проекты, информации ноль кто чего согласовал, какие проекты открыты и кто их ведет. Вообще информации ноль!от Миши Б:
1. SR по сверке ОМС UK против Калипсо так пока и не заведен, несмотря на то, что Наташей Рахмановой отсутствие данной  сверки было заявлено как show-stopper для отключения прогрузки сделок UK в К+.
1. Перевод фондирования в КХД и отказ от фондирования UK - нет ответа по статусу этих вопросов.
1. Статус определения системы для Казны (предложенное решение - Атриум) - не известен.

От Кости Е.<ul><li>BBG CY certificate is about to expire, KHD team informed</li><li>No possibility yet to setup Grafana minitoring at EP</li></ul> | 







*****

[[category.storage-team]] 
[[category.confluence]] 
