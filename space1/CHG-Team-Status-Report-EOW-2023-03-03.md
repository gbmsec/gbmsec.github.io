





| CHG

 | 
| Alexey Dorogov

 | 
| 

 | 
| CRM

1) CRM для Non-UK - Проработка вариантов SF-thru-CY/ELMA (CRM+BPM) 2) Коммуникация с Conga и FormAssembley - исправление счета FormAssembley, подготовка к миграции кипрского функционала FA на орг в KZ, откладывание вопроса приобретения Conga 3) Регистрация интеграций Salesforce 4) Добавление кипрского адреса CRM в адреса рассылки системы и установка его для всех рассылок по кипрским счетам и клиентам 5) Интеграция с Калипсо - наполнение историческими данными полей с кодами стран, входящих в скоуп интеграции



Calypso:

<ul><li>Продолжаем тестирование на UAT и PREP  **июльской** версией Калипсо 16.22.7.3 Активное участие пользователей приводит к нахождению багов, которые мы оперативно пытаемся чинить, чтобы успеть все исправить к релизу.</li><li>Загрузка сделок из BBG TOMS - задачи в разработке на ESB и команде Calypso.</li><li>Загрузка сделок из OMS Quick - пытаемся настроить подключение, чтобы начали приходить экзекьюшены.</li><li>По CASS проекту идет UAT тестирования уже реализованной функциональности. </li><li>По клиентским зеркалам задачи ждут релиза Калипсо, чтобы можно было начать делать исправления в PROD.</li><li>MiFID Post Trade Reporting - продолжаем делать аналитику, но встал вопрос еще раз пересмотреть архитектуру решения, чтобы репортинг делался из FO части, а не BO.</li></ul>IBQ:

<ul><li>Работаем над текущими задачами. Багфиксинг критичных ошибок и начали работу по критичным SR. Работы по сегрегации IBQ и сервисов пока на паузе, но предварительные работы уже начаты.</li><li>Начали чистку папок на FTP. Большую часть файлов уже удалили.</li><li>Анализ по разделению сервиса OneTick закончен, ждем ресурс разработки.</li><li>Анализ по сегрегации SFTR и Reg Reporting Service в процессе.</li><li>Отключили согласованные с OPS загрузки на обработку файлов в IBQ.</li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>ESB Segregation: Migration to Kubernetes - NonUK</li><li>ESB Segregation: nonUK UAT infrastructure </li></ul>RRTTCA CY: mvp is in prod, loading missing prices from quik added Still having an issue with Bond pricing form Quik is different from BBG, waiting Dm. Arshevsky to clarify FX: started to setup test env; new task added for NDF processing - in progress UK/non UK: started to move repository, waiting copy of nuget repositories to proceed started to setup YA dev env., waiting for other apps to integrate with Refactoring: Ilya presented new data scheme for instruments and pricesKondor
1. Транспорт ЛЗ Казны переведен на КХД, также в КХД теперь проводятся все расчеты по графикам и процентам по всем займам.
1. Из-за производительности нового HW К+ в Москве было принято решение о размещении его на СХД. Сроки переезда сдвигаются.
1. От Систематики получен допник по работе с аффелированными компаниями (пока оказалось критично для БКС Дубаи).

 | 
| top 3-5 points | 
| 1) IBQ resources2) HR data quality in Click HR3) Kuber status and issues:<ul><li>SMB Mount - in progress (driver installed working with parameters to correct mounting storage)</li><li>Nuget repositories - done.</li><li>Consul - bugs in official helm chart  app runs not correctly (in parallel try to use ConfigMaps in apps)</li><li>Vault - plan to deploy</li><li>Keycloak authentication, import realms, roles, users, clients from UK?</li></ul> | 
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

1) CRM для Non-UK - Проработка вариантов SF-thru-CY/ELMA (CRM+BPM) 2) Коммуникация с Conga и FormAssembley - исправление счета FormAssembley, подготовка к миграции кипрского функционала FA на орг в KZ, откладывание вопроса приобретения Conga 3) Регистрация интеграций Salesforce 4) Добавление кипрского адреса CRM в адреса рассылки системы и установка его для всех рассылок по кипрским счетам и клиентам 5) Интеграция с Калипсо - наполнение историческими данными полей с кодами стран, входящих в скоуп интеграции



Calypso:

<ul><li>Продолжаем тестирование на UAT и PREP  **июльской** версией Калипсо 16.22.7.3 Активное участие пользователей приводит к нахождению багов, которые мы оперативно пытаемся чинить, чтобы успеть все исправить к релизу.</li><li>Загрузка сделок из BBG TOMS - задачи в разработке на ESB и команде Calypso.</li><li>Загрузка сделок из OMS Quick - пытаемся настроить подключение, чтобы начали приходить экзекьюшены.</li><li>По CASS проекту идет UAT тестирования уже реализованной функциональности. </li><li>По клиентским зеркалам задачи ждут релиза Калипсо, чтобы можно было начать делать исправления в PROD.</li><li>MiFID Post Trade Reporting - продолжаем делать аналитику, но встал вопрос еще раз пересмотреть архитектуру решения, чтобы репортинг делался из FO части, а не BO.</li></ul>IBQ:

<ul><li>Работаем над текущими задачами. Багфиксинг критичных ошибок и начали работу по критичным SR. Работы по сегрегации IBQ и сервисов пока на паузе, но предварительные работы уже начаты.</li><li>Начали чистку папок на FTP. Большую часть файлов уже удалили.</li><li>Анализ по разделению сервиса OneTick закончен, ждем ресурс разработки.</li><li>Анализ по сегрегации SFTR и Reg Reporting Service в процессе.</li><li>Отключили согласованные с OPS загрузки на обработку файлов в IBQ.</li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>ESB Segregation: Migration to Kubernetes - NonUK</li><li>ESB Segregation: nonUK UAT infrastructure </li></ul>RRTTCA CY: mvp is in prod, loading missing prices from quik added Still having an issue with Bond pricing form Quik is different from BBG, waiting Dm. Arshevsky to clarify FX: started to setup test env; new task added for NDF processing - in progress UK/non UK: started to move repository, waiting copy of nuget repositories to proceed started to setup YA dev env., waiting for other apps to integrate with Refactoring: Ilya presented new data scheme for instruments and pricesKondor
1. Транспорт ЛЗ Казны переведен на КХД, также в КХД теперь проводятся все расчеты по графикам и процентам по всем займам.
1. Из-за производительности нового HW К+ в Москве было принято решение о размещении его на СХД. Сроки переезда сдвигаются.
1. От Систематики получен допник по работе с аффелированными компаниями (пока оказалось критично для БКС Дубаи).

 | 
| top 3-5 points | 
| 1) IBQ resources2) HR data quality in Click HR3) Kuber status and issues:<ul><li>SMB Mount - in progress (driver installed working with parameters to correct mounting storage)</li><li>Nuget repositories - done.</li><li>Consul - bugs in official helm chart  app runs not correctly (in parallel try to use ConfigMaps in apps)</li><li>Vault - plan to deploy</li><li>Keycloak authentication, import realms, roles, users, clients from UK?</li></ul> | 







*****

[[category.storage-team]] 
[[category.confluence]] 
