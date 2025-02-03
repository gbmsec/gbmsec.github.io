





| CHG

 | 
| 

 | 
| 

 | 
| Calypso<ul><li>По CASS проекту продолжается попродуктовое тестирование и UAT.  Проблему с SDI решили. Продолжаем тестирования инструкцтирование. Прорабатываем требования по Fees и Nettings.</li><li>Начали прорабатывать требования на загрузку сделок напрямую в Calypso, а также вопросы по формированию MiFID Post Trade Reporting.</li></ul>IBQ:

<ul><li>Успешно закончилость тестирование в рамках проекта TTCA. После выхода релиза по RR необходимо будет заполнить справочник мапинга счетов в IBQ,</li><li>В рамках подготовки нового квартального отчета CA-CIF по Кипру столкнулись с проблемой загрузки статики из Sales Force. Для решения выпустили хотфикс на ESB. Данные были собраны и предоставлены.</li><li>Ждем когда инфраструктура предоставит нам сервера для миграции QORT / IBQ из UK контура. Обновили план миграции по QORT и добавили часть работ по IBQ.</li></ul> **RR** CASS: No activities at RR sideTTCA  CY: started integration testing with Calypso, some fixes are done, also new request to Calypso is raisedFX: waiting IBSO development to test integration, also they need to setup test envDBAs raised request to open database ports from dev/prod KHD, need a project arch diagramUK/non UK:<ul><li>move databases from azr-rr-dev1 to dcix-dailydb: db is ready, need to plan moving, win services stay where they are (only billing is going to change), need to change SQL license on current AZR</li><li>discussion how to migrate equity report to calypso data for uk (Mikhail Rakov): Calypso is already sending some data for Finance. One of the options to keep risk parameters of that report in RR</li><li>started to setup YA dev env., waiting for other apps to integrate with</li></ul>Refactoring:<ul><li>Dev started for K+ integration to ESB</li><li>2 SSIS packages replacements went to RPOD</li></ul>SR and other tasks: New requests to investigate/fix some numbers in MC Repo room, and TTCA CY Balances reportESB<ul><li>ESB internal tasks and bugs</li><li>Migration to Kubernetes - NonUK</li><li>Pershing CUSIP-ISIN cache</li></ul>Kondor
1. Начался тест процедуры перевода транспорта ЛЗ на КХД.
1. Выведена в прод возможность отключения экспортеров в шлюзе забора маркет цен (сегрегация).
1. Переезд К+ обратно в Москву: stunnel переброшен на отдельную виртуалку, выполнена СЗ по открытию доступа групповых пользователей к новому Радиусу, установлен Sybase DR сервер, в отладке процедура синхронизации.
1. Встреча с Казначейством: грозятся перевести все фондирование в КХД (Станиславксий: "Не верю."), в связи с чем принято решение пока не проводить ежегодную процедуру "обрезания" больших позиций
1. Определен вектор дальнейшего движения по найму аналитика: есть варианты, прорабатываем с HR.
1. Исправлена "ошибка" по "некорректной" передаче графиков ЛЗ, переходящих через год, в КХД. Теперь в 1С смогут закрыть год.
1. Вывели SR по загрузке американских сделок.

 | 
| top 3-5 points | 
| 
1. Хрень по FX
1.  численность по командам - юк - нон-юк

 | 
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
| Calypso<ul><li>По CASS проекту продолжается попродуктовое тестирование и UAT.  Проблему с SDI решили. Продолжаем тестирования инструкцтирование. Прорабатываем требования по Fees и Nettings.</li><li>Начали прорабатывать требования на загрузку сделок напрямую в Calypso, а также вопросы по формированию MiFID Post Trade Reporting.</li></ul>IBQ:

<ul><li>Успешно закончилость тестирование в рамках проекта TTCA. После выхода релиза по RR необходимо будет заполнить справочник мапинга счетов в IBQ,</li><li>В рамках подготовки нового квартального отчета CA-CIF по Кипру столкнулись с проблемой загрузки статики из Sales Force. Для решения выпустили хотфикс на ESB. Данные были собраны и предоставлены.</li><li>Ждем когда инфраструктура предоставит нам сервера для миграции QORT / IBQ из UK контура. Обновили план миграции по QORT и добавили часть работ по IBQ.</li></ul> **RR** CASS: No activities at RR sideTTCA  CY: started integration testing with Calypso, some fixes are done, also new request to Calypso is raisedFX: waiting IBSO development to test integration, also they need to setup test envDBAs raised request to open database ports from dev/prod KHD, need a project arch diagramUK/non UK:<ul><li>move databases from azr-rr-dev1 to dcix-dailydb: db is ready, need to plan moving, win services stay where they are (only billing is going to change), need to change SQL license on current AZR</li><li>discussion how to migrate equity report to calypso data for uk (Mikhail Rakov): Calypso is already sending some data for Finance. One of the options to keep risk parameters of that report in RR</li><li>started to setup YA dev env., waiting for other apps to integrate with</li></ul>Refactoring:<ul><li>Dev started for K+ integration to ESB</li><li>2 SSIS packages replacements went to RPOD</li></ul>SR and other tasks: New requests to investigate/fix some numbers in MC Repo room, and TTCA CY Balances reportESB<ul><li>ESB internal tasks and bugs</li><li>Migration to Kubernetes - NonUK</li><li>Pershing CUSIP-ISIN cache</li></ul>Kondor
1. Начался тест процедуры перевода транспорта ЛЗ на КХД.
1. Выведена в прод возможность отключения экспортеров в шлюзе забора маркет цен (сегрегация).
1. Переезд К+ обратно в Москву: stunnel переброшен на отдельную виртуалку, выполнена СЗ по открытию доступа групповых пользователей к новому Радиусу, установлен Sybase DR сервер, в отладке процедура синхронизации.
1. Встреча с Казначейством: грозятся перевести все фондирование в КХД (Станиславксий: "Не верю."), в связи с чем принято решение пока не проводить ежегодную процедуру "обрезания" больших позиций
1. Определен вектор дальнейшего движения по найму аналитика: есть варианты, прорабатываем с HR.
1. Исправлена "ошибка" по "некорректной" передаче графиков ЛЗ, переходящих через год, в КХД. Теперь в 1С смогут закрыть год.
1. Вывели SR по загрузке американских сделок.

 | 
| top 3-5 points | 
| 
1. Хрень по FX
1.  численность по командам - юк - нон-юк

 | 







*****

[[category.storage-team]] 
[[category.confluence]] 
