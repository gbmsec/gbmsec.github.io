





| CHG

 | 
| 

 | 
|    

 | 
| Получили письмо от SF с запросом что за сервисы установлены в России. Есть риски, что могут не продлить на 23 год

ESB

<ul><li>ESB internal tasks and bugs</li><li>Migration to Kubernetes</li><li>Segregation flows diagrams</li><li>MOEX → Calypso integration</li></ul>Calypso:

<ul><li>Продолжается тестирование новой версии Calypso 16.22.7.3, работаем над ошибками связанными с Bloomberg. На текущий момент успешно пройдено 99% из тестов Вадима. Осталось разобрать ошибки по Trade Confo.</li><li>По CASS провели провели встречу по новому репортингу в FCA. Обсудили необходимые данные для построения отчета и какие системы могут их предоставить. Репортинг ежемесячный, планируем делать реализацию в Calypso</li><li>Продолжается активная работа по доработкам интеграции и сверок для выверки данных между SalesForce и Calypso в рамках тестирования.</li></ul>Kondor
1. Загрузили новые признаки к счетам. Теперь нужно приступать к анализу.
1. Вывели загрузку 0-го НКД по всем сделкам - чтобы такие сделки грузились бы сразу, не падая в ошибки.
1. С большой долей вероятности К+ все-таки должен переехать в Россию. Обсудили с инфраструктурой - вроде по железу можем это сделать.
1. Казначейство - на следующей неделе перевода транспорта ЛЗ на КХД не будет - не закончено тестирование. Новый срок - неделя с 12.12. По переводу транспорта P&L сплитов наших Finance со стороны бизнеса (Евгения Сычева) пришел запрос, что этого делать не надо. Запланирована встреча.
1. Еще у нескольких ролей отозван доступ к счетам Кипра. По многим пользователи выясняют их присутствие в договорах ОА - и как туда попасть...
1. ЕР - с нашей стороны на проде все готово, но "тестовой" сделки пока не случилось. Ожидается на следующей неделе.
1. В этом релизе запланирован вывод задачи по изменению структуры FIX сообщений NT-Pro, которая является show-stopper для перехода на новый транспорт post-trade репортинга.

RRCASS: preparation for project UAT, tune CASS UI behavior when sending transfers (no Amends/Cancels to Calypso) FX: fix some cosmetics, analyze new requirementsSL3: fix hardcoded notification start; sorted out CY exporters diffUK/non UK:<ul><li>presented draft UK Risks architecture </li><li>investigate bbg connection thru CY</li></ul>Refactoring:<ul><li>succeeded to send messages from ms sql to rabbitmq</li><li>setup rabbit mq cluster at dev (azr1&2)</li></ul> | 
| top 3-5 points | 
|  | 
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
| Получили письмо от SF с запросом что за сервисы установлены в России. Есть риски, что могут не продлить на 23 год

ESB

<ul><li>ESB internal tasks and bugs</li><li>Migration to Kubernetes</li><li>Segregation flows diagrams</li><li>MOEX → Calypso integration</li></ul>Calypso:

<ul><li>Продолжается тестирование новой версии Calypso 16.22.7.3, работаем над ошибками связанными с Bloomberg. На текущий момент успешно пройдено 99% из тестов Вадима. Осталось разобрать ошибки по Trade Confo.</li><li>По CASS провели провели встречу по новому репортингу в FCA. Обсудили необходимые данные для построения отчета и какие системы могут их предоставить. Репортинг ежемесячный, планируем делать реализацию в Calypso</li><li>Продолжается активная работа по доработкам интеграции и сверок для выверки данных между SalesForce и Calypso в рамках тестирования.</li></ul>Kondor
1. Загрузили новые признаки к счетам. Теперь нужно приступать к анализу.
1. Вывели загрузку 0-го НКД по всем сделкам - чтобы такие сделки грузились бы сразу, не падая в ошибки.
1. С большой долей вероятности К+ все-таки должен переехать в Россию. Обсудили с инфраструктурой - вроде по железу можем это сделать.
1. Казначейство - на следующей неделе перевода транспорта ЛЗ на КХД не будет - не закончено тестирование. Новый срок - неделя с 12.12. По переводу транспорта P&L сплитов наших Finance со стороны бизнеса (Евгения Сычева) пришел запрос, что этого делать не надо. Запланирована встреча.
1. Еще у нескольких ролей отозван доступ к счетам Кипра. По многим пользователи выясняют их присутствие в договорах ОА - и как туда попасть...
1. ЕР - с нашей стороны на проде все готово, но "тестовой" сделки пока не случилось. Ожидается на следующей неделе.
1. В этом релизе запланирован вывод задачи по изменению структуры FIX сообщений NT-Pro, которая является show-stopper для перехода на новый транспорт post-trade репортинга.

RRCASS: preparation for project UAT, tune CASS UI behavior when sending transfers (no Amends/Cancels to Calypso) FX: fix some cosmetics, analyze new requirementsSL3: fix hardcoded notification start; sorted out CY exporters diffUK/non UK:<ul><li>presented draft UK Risks architecture </li><li>investigate bbg connection thru CY</li></ul>Refactoring:<ul><li>succeeded to send messages from ms sql to rabbitmq</li><li>setup rabbit mq cluster at dev (azr1&2)</li></ul> | 
| top 3-5 points | 
|  | 







*****

[[category.storage-team]] 
[[category.confluence]] 
