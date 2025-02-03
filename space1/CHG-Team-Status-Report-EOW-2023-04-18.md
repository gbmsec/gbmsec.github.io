





| CHG

 | 
| Alexey Dorogov

 | 
| 

 | 
| CRM

1) CRS Reporting actualization - работы по перенастройке полей системы в рамках REQ-1837

2) Integration with Calypso - тестирование интеграции Tax Cases, а также подготовка обновления исторических данных нововведёнными параметрами.

3) CRM Non-UK

<ul><li>Проведена встреча с BPM-Soft</li><li>Заданы дополнительные вопросы</li><li>Создан и пополняется информацией сводный файл со сравнением с скорингом для вендоров по всем интересующим параметрам</li><li>Перепроверены варианты сетапа с СФ и подтверждено присутствие тех или иных рисков для всех вариантов.</li></ul>4) Выверка справочных данных по ЦФО между Salesforce и КХД



Кондор


1. С точки зрения nonUK финансового департамента show-stopper-ов по прекращению загрузки сделок UK в К+ нет.
1. Послан запрос-предупреждение пользователям на отключение позиций (как объектов позиционного движка), которые содержат сделки как UK, так и nonUK. 
1. Получен список открытых в Qort счетов - для проведения анализа прав в К+ по запросу compliance Кипра.
1. ТОМС сейчас не используется на Кипре, эта задача не show-stopper для сегрегации. Запрошен SR на автоматизацию потока VCON.
1. PostTrade репортинг - найдена брешь в оценке бирж (например, наших) - надо ли по ним репортить сделки Кипра. Получен SR.
1. Актуализируем с прода тест 2 - девелоперская среда.

Calypso:

<ul><li>По CASS проекту получили список задач, которые мы оценили в 75MD, ждем подтверждение, что эти задачи нужно реализовать.</li><li>MiFID Post Trade Reporting - ведем разработку.</li><li>После архитектурного комитета по проектам Calypso Non UK был вопрос по персонифицированной аутентификации в Calypso Non UK. На схеме архитектуры оставили Calypso авторизацию. Вопрос использования windows или sso заявлены, в качестве альтернативы.</li></ul>IBQ:

<ul><li>Делаем сетап IBQ на новых серверах Кипра</li><li>Делаем переносу FTD Notes в Non UK кубер</li></ul>Нарисовали архитектуру по Reg Reporting Service в Non UK контуре для запуска проекта EMIR Refit

РР

FX: testing in progress

UK/non UK:

<ul><li>testing and setting up UK SE database env, DBAs took decision to go with 2019 version, not 2022</li><li>continue deploying services to EP k8s UAT</li><li>decision on RuData to be taken (Robert is searching for budgeting)</li><li>access requests to KHD from EP were raised, are in progress still</li><li>K+ flows split on K+ level is agreed, list of necessary queues was provided</li><li>UI is splitted</li></ul>Refactoring: ODS load - proceeded, K+ loader is in progress, need to switch development to EP, but no test data there. Need to clarify further also, as the logic is changed

ESB<ul><li>ESB internal tasks and bugs</li><li>ESB Segregation: Migration to Kubernetes - NonUK</li><li>ESB Segregation: nonUK UAT infrastructure</li></ul> | 
| top 3-5 points | 
| 
1. Не можем начать ЮАТ РР - нет учеток в домене ЕП
1. пользаки Калипсо - выше лимита пока
1.  ОПС затягивает с ответом по отключению контура Т-1 на ЮК, а нам нужно освободить инфру, не называют дату
1. Кубер - нет доступов в НТПро, задерживаем KeyCloack
1.  **!!!!**  Есть задержка на 4 дня по работе с Кубером из-за реаллокации Ромы В. на срочную задачу по автоматизации рег репортинга Emir FX FW для Дубая - [IBQ-5430 BCS IB JIRA](https:///browse/IBQ-5430)

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
| CRM

1) CRS Reporting actualization - работы по перенастройке полей системы в рамках REQ-1837

2) Integration with Calypso - тестирование интеграции Tax Cases, а также подготовка обновления исторических данных нововведёнными параметрами.

3) CRM Non-UK

<ul><li>Проведена встреча с BPM-Soft</li><li>Заданы дополнительные вопросы</li><li>Создан и пополняется информацией сводный файл со сравнением с скорингом для вендоров по всем интересующим параметрам</li><li>Перепроверены варианты сетапа с СФ и подтверждено присутствие тех или иных рисков для всех вариантов.</li></ul>4) Выверка справочных данных по ЦФО между Salesforce и КХД



Кондор


1. С точки зрения nonUK финансового департамента show-stopper-ов по прекращению загрузки сделок UK в К+ нет.
1. Послан запрос-предупреждение пользователям на отключение позиций (как объектов позиционного движка), которые содержат сделки как UK, так и nonUK. 
1. Получен список открытых в Qort счетов - для проведения анализа прав в К+ по запросу compliance Кипра.
1. ТОМС сейчас не используется на Кипре, эта задача не show-stopper для сегрегации. Запрошен SR на автоматизацию потока VCON.
1. PostTrade репортинг - найдена брешь в оценке бирж (например, наших) - надо ли по ним репортить сделки Кипра. Получен SR.
1. Актуализируем с прода тест 2 - девелоперская среда.

Calypso:

<ul><li>По CASS проекту получили список задач, которые мы оценили в 75MD, ждем подтверждение, что эти задачи нужно реализовать.</li><li>MiFID Post Trade Reporting - ведем разработку.</li><li>После архитектурного комитета по проектам Calypso Non UK был вопрос по персонифицированной аутентификации в Calypso Non UK. На схеме архитектуры оставили Calypso авторизацию. Вопрос использования windows или sso заявлены, в качестве альтернативы.</li></ul>IBQ:

<ul><li>Делаем сетап IBQ на новых серверах Кипра</li><li>Делаем переносу FTD Notes в Non UK кубер</li></ul>Нарисовали архитектуру по Reg Reporting Service в Non UK контуре для запуска проекта EMIR Refit

РР

FX: testing in progress

UK/non UK:

<ul><li>testing and setting up UK SE database env, DBAs took decision to go with 2019 version, not 2022</li><li>continue deploying services to EP k8s UAT</li><li>decision on RuData to be taken (Robert is searching for budgeting)</li><li>access requests to KHD from EP were raised, are in progress still</li><li>K+ flows split on K+ level is agreed, list of necessary queues was provided</li><li>UI is splitted</li></ul>Refactoring: ODS load - proceeded, K+ loader is in progress, need to switch development to EP, but no test data there. Need to clarify further also, as the logic is changed

ESB<ul><li>ESB internal tasks and bugs</li><li>ESB Segregation: Migration to Kubernetes - NonUK</li><li>ESB Segregation: nonUK UAT infrastructure</li></ul> | 
| top 3-5 points | 
| 
1. Не можем начать ЮАТ РР - нет учеток в домене ЕП
1. пользаки Калипсо - выше лимита пока
1.  ОПС затягивает с ответом по отключению контура Т-1 на ЮК, а нам нужно освободить инфру, не называют дату
1. Кубер - нет доступов в НТПро, задерживаем KeyCloack
1.  **!!!!**  Есть задержка на 4 дня по работе с Кубером из-за реаллокации Ромы В. на срочную задачу по автоматизации рег репортинга Emir FX FW для Дубая - [IBQ-5430 BCS IB JIRA](https:///browse/IBQ-5430)

 | 







*****

[[category.storage-team]] 
[[category.confluence]] 
