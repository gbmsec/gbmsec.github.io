





| CHG

 | 
| Alexey Dorogov

 | 
| 

 | 
| Riskroom:

<ul><li>RuData connectivity verified, started working on a service</li><li>ARM RM FOP limits calculation development is ongoing</li><li>Got more data on Bonds from Calypso, need to integrate</li></ul>FX:

<ul><li>Emergency console rates stopping bug fix is done</li><li>FINAM report: UAT is ongoing, waiting feedback from customer</li><li>Emergency dashboard bug fix is at PROD</li><li>Started working on adding 2 fields onto Emergency dashboard warning</li></ul>OneTick:

<ul><li>delivered functionality for EP to unload files into separate folders by year for OneTick historical data request</li></ul>

Calypso:

<ul><li>Продолжаем занимаемся задачей по переходу с FIX сообщений на загрузку из QUIK экспортера. Есть вопросы, которые бы хотелось совместно с командой FO и ESB решить.</li><li>Calypso Non UK - обсудили начало тестирования интеграций в тестовой среде PREPCY. Определили список интеграций подлежащий тестированию. Составляем тестовые сценарии. Обсудили интеграции с ESB, SF, ОХД особенно в части распараллеливания публикации статики из UK и Non UK.</li><li>Декомиссия Kondor+ в периметре UK - выводим в релиз  исправления и доработки по репортингу MiFID PostTrade в TradeECHO. Делали исправления по загрузке сделок напрямую в Calypso. По сверкам выводим в релиз сверки со стороны Калипсо (TOMS и OMS). Дополнительно исправили проблему с отображение данных для трейдеров деска в Position Keeper.</li><li>CASS - продолжаем попродуктовое тестирование и исправление ошибок. </li></ul>

IBQ:

<ul><li>Делаем аналитику по проекту EMIR Refit. Готово описание по FX Forward, можем начинать предварительные работы со стороны разработки.</li><li>По OT в рамках договоренностей с Комплаенс UK перевыгрузили необходимые данные за 2022 год. Остается очень большой объем на выгрузку за 2021 год.</li></ul>Кондор
1. Подписаны ДС-ы с Систематикой на переход на Атриум.
1. уходит Коля Дружинин - что ставит проект перехода под большой ресурсный риск.
1. Можно сказать, что Тест 2 окончательно прижился в Москве и не зависит от Лондона. Решен вопрос с лицензионным файлом, сейчас срок действия до конца 2024 (как и всего К+).
1. Деактивировали пользователя РР в базе данных - окончательно ушли от интеграции с ними через db-link.
1. Прошла встреча по Agile, финализирующая итоги 3-го квартала.
1. Согласовали с FX desk внедрение новой архитектуры взаимодействия с NT-Pro (фильтрация на нашей стороне) без их UAT из-за его сложности. QA, естественно, планируется.

 | 
| top 3-5 points | 
| 1) HR - все плохо, позитивных новостей или сдвигов нет2) PRJ 310 Emir refit - плохо. И. Медведева уходит. Коммуникации не было. БРД не доделан, абсолютно сырой. Срок подготовки проектных документов тоже прошел, но теперь без Иры непонятно кто и как их будет делать. С нашей стороны разработку еще не начали, но готовимся, обсуждения провели.3) Актуальный список задач на Инфра - key in (INFRA-4077, INFRA-3323, INFRA-3775, INFRA-4086, INFRA-2661, INFRA-2060, INFRA-4103, INFRA-4244, INFRA-4224, INFRA-3654, INFRA-4223, INFRA-4153, INFRA-4151, INFRA-4151, INFRA-4293, INFRA-4318, INFRA-4238, INFRA-4360, INFRA-4300, INFRA-4254, INFRA-4372, INFRA-4384) | 
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
| Riskroom:

<ul><li>RuData connectivity verified, started working on a service</li><li>ARM RM FOP limits calculation development is ongoing</li><li>Got more data on Bonds from Calypso, need to integrate</li></ul>FX:

<ul><li>Emergency console rates stopping bug fix is done</li><li>FINAM report: UAT is ongoing, waiting feedback from customer</li><li>Emergency dashboard bug fix is at PROD</li><li>Started working on adding 2 fields onto Emergency dashboard warning</li></ul>OneTick:

<ul><li>delivered functionality for EP to unload files into separate folders by year for OneTick historical data request</li></ul>

Calypso:

<ul><li>Продолжаем занимаемся задачей по переходу с FIX сообщений на загрузку из QUIK экспортера. Есть вопросы, которые бы хотелось совместно с командой FO и ESB решить.</li><li>Calypso Non UK - обсудили начало тестирования интеграций в тестовой среде PREPCY. Определили список интеграций подлежащий тестированию. Составляем тестовые сценарии. Обсудили интеграции с ESB, SF, ОХД особенно в части распараллеливания публикации статики из UK и Non UK.</li><li>Декомиссия Kondor+ в периметре UK - выводим в релиз  исправления и доработки по репортингу MiFID PostTrade в TradeECHO. Делали исправления по загрузке сделок напрямую в Calypso. По сверкам выводим в релиз сверки со стороны Калипсо (TOMS и OMS). Дополнительно исправили проблему с отображение данных для трейдеров деска в Position Keeper.</li><li>CASS - продолжаем попродуктовое тестирование и исправление ошибок. </li></ul>

IBQ:

<ul><li>Делаем аналитику по проекту EMIR Refit. Готово описание по FX Forward, можем начинать предварительные работы со стороны разработки.</li><li>По OT в рамках договоренностей с Комплаенс UK перевыгрузили необходимые данные за 2022 год. Остается очень большой объем на выгрузку за 2021 год.</li></ul>Кондор
1. Подписаны ДС-ы с Систематикой на переход на Атриум.
1. уходит Коля Дружинин - что ставит проект перехода под большой ресурсный риск.
1. Можно сказать, что Тест 2 окончательно прижился в Москве и не зависит от Лондона. Решен вопрос с лицензионным файлом, сейчас срок действия до конца 2024 (как и всего К+).
1. Деактивировали пользователя РР в базе данных - окончательно ушли от интеграции с ними через db-link.
1. Прошла встреча по Agile, финализирующая итоги 3-го квартала.
1. Согласовали с FX desk внедрение новой архитектуры взаимодействия с NT-Pro (фильтрация на нашей стороне) без их UAT из-за его сложности. QA, естественно, планируется.

 | 
| top 3-5 points | 
| 1) HR - все плохо, позитивных новостей или сдвигов нет2) PRJ 310 Emir refit - плохо. И. Медведева уходит. Коммуникации не было. БРД не доделан, абсолютно сырой. Срок подготовки проектных документов тоже прошел, но теперь без Иры непонятно кто и как их будет делать. С нашей стороны разработку еще не начали, но готовимся, обсуждения провели.3) Актуальный список задач на Инфра - key in (INFRA-4077, INFRA-3323, INFRA-3775, INFRA-4086, INFRA-2661, INFRA-2060, INFRA-4103, INFRA-4244, INFRA-4224, INFRA-3654, INFRA-4223, INFRA-4153, INFRA-4151, INFRA-4151, INFRA-4293, INFRA-4318, INFRA-4238, INFRA-4360, INFRA-4300, INFRA-4254, INFRA-4372, INFRA-4384) | 







*****

[[category.storage-team]] 
[[category.confluence]] 
