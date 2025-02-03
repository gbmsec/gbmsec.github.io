





| CHG

 | 
| Alexey Dorogov

 | 
|    

 | 
| EDW

<ul><li>Oracle 19 testing</li><li>Monitoring</li><li>Bug Classification</li><li>SCS - QUIK integration</li><li>SCS - Split technical and bisness sanction lists</li><li>Change logic upload rates from KHD</li></ul>Calypso

<ul><li>  Планируем миграцию книг по проекту Trading Books restructuring</li><li>Денис продолжает чистку аудита по po_postings, скорость оч маленькая. 1 месяц мы чистим за 12 дней по времени. Так что все работы растягиваются. Остается чистить еще месяцев 15 на текущий момент.</li></ul>RR

<ul><li>continue development for Intraday limits, tech and business tasks</li></ul>Kondor


1.  Market data через Trep (в К+ и Квик) пока поставляется, но риск западных провайдеров остается. Поговорили с Систематикой - у них есть адаптеры на получение MD в К+ из Квик, excel,  **Прайм** .
1. Отключили "мертвые" души, после чего провели ревизию к-ва лицензий по ролям. Для equities и FI десков к-во лицензий превышает к-во пользователей. FI деск, в лице Сергея Федорова, уже позволил высвободить 4 лицензии.
1. Подняли старую тему чистки не используемых позиций Equities деска. Проговорили дальнейшие шаги по определению, что же используется.
1. Проект ведения брокерского бизнеса - принято решение отказаться от Калипсо как БО. Пока не ясна судьба задач на К+ в этом проекте.
1. Большинство проектов ушло на холд. Также как и вопрос по закупке лицензий Систематика Радиус.
1. посмотрим по серверам, которые закупали ранее под миграцию, определим те, которые не потребуются, передадим в srv для использования

CPORT


1. Небольшой фикс по калькулятору индекса в hnwi портале
1. Начали подключение к keycloack
1. Изменили шаблон писем для рассылки ресерч отчетов



FX
1. Выносим настройки переключения источников котировок в GUI Emergency, на следующей неделе планируем UAT
1. Документация по сервисам Synthetic Quotes, Volatility calc
1. Приведение в порядок дашбордов FX Desk сервисов

CRM 1) Finalizing Profile migration 2) LEI parser/collector - preliminary analysis 3) Research Page - contact rating implementation 4) EMIR/SFTR - preparation of sample data files, discussions on upcoming changes with EDW 5) Vendor blockage - discussing SF with vendor, all seems fine for now with positive prediction 6) bugfixes | 
| top 3-5 points | 
| Обсудить идею перехода на дополнительные поставщики данных, например сервис Ru Data от ИнтерфаксНужно определить стратегию по поставщику Market Data | 
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
| EDW

<ul><li>Oracle 19 testing</li><li>Monitoring</li><li>Bug Classification</li><li>SCS - QUIK integration</li><li>SCS - Split technical and bisness sanction lists</li><li>Change logic upload rates from KHD</li></ul>Calypso

<ul><li>  Планируем миграцию книг по проекту Trading Books restructuring</li><li>Денис продолжает чистку аудита по po_postings, скорость оч маленькая. 1 месяц мы чистим за 12 дней по времени. Так что все работы растягиваются. Остается чистить еще месяцев 15 на текущий момент.</li></ul>RR

<ul><li>continue development for Intraday limits, tech and business tasks</li></ul>Kondor


1.  Market data через Trep (в К+ и Квик) пока поставляется, но риск западных провайдеров остается. Поговорили с Систематикой - у них есть адаптеры на получение MD в К+ из Квик, excel,  **Прайм** .
1. Отключили "мертвые" души, после чего провели ревизию к-ва лицензий по ролям. Для equities и FI десков к-во лицензий превышает к-во пользователей. FI деск, в лице Сергея Федорова, уже позволил высвободить 4 лицензии.
1. Подняли старую тему чистки не используемых позиций Equities деска. Проговорили дальнейшие шаги по определению, что же используется.
1. Проект ведения брокерского бизнеса - принято решение отказаться от Калипсо как БО. Пока не ясна судьба задач на К+ в этом проекте.
1. Большинство проектов ушло на холд. Также как и вопрос по закупке лицензий Систематика Радиус.
1. посмотрим по серверам, которые закупали ранее под миграцию, определим те, которые не потребуются, передадим в srv для использования

CPORT


1. Небольшой фикс по калькулятору индекса в hnwi портале
1. Начали подключение к keycloack
1. Изменили шаблон писем для рассылки ресерч отчетов



FX
1. Выносим настройки переключения источников котировок в GUI Emergency, на следующей неделе планируем UAT
1. Документация по сервисам Synthetic Quotes, Volatility calc
1. Приведение в порядок дашбордов FX Desk сервисов

CRM 1) Finalizing Profile migration 2) LEI parser/collector - preliminary analysis 3) Research Page - contact rating implementation 4) EMIR/SFTR - preparation of sample data files, discussions on upcoming changes with EDW 5) Vendor blockage - discussing SF with vendor, all seems fine for now with positive prediction 6) bugfixes | 
| top 3-5 points | 
| Обсудить идею перехода на дополнительные поставщики данных, например сервис Ru Data от ИнтерфаксНужно определить стратегию по поставщику Market Data | 







*****

[[category.storage-team]] 
[[category.confluence]] 
