





| CHG

 | 
| Alexey Dorogov

 | 
|  

 | 
| Kondor
1. Продолжаем совместно с другими командами работать над проблемой экспортеров. 
1. В этом релизе запланирован вывод последней задачи на стороне К+ проекта NT-Pro.
1. Была проведена ознакомительная встреча с обновленной Казной. Познакомились. Далее будем координировать в рабочем порядке. Про проект перевода фондирования, который ведет Рохлина, они знают.
1. Вывели в прод одну из задач OPS Efficiency по сверкам - репо. "-й день, полет нормальный.

CPORT
1. Задачи по ресерч порталу - улучшение работы фильтров, добавление новых
1. Отчитались о результатах спринта коллегам из ресерч

EDW<ul><li>SCS. Add filter into ssi reference rules on field country_id</li><li>SCS. E-Disclosure notification</li><li>Portfolio reconciliation</li><li>SFTR Reconciliation in Reg Reporting Service</li><li>FX Option</li></ul>CRM<ul><li>Pre-analysis for Digital Communications Channels Project</li><li>FormAssembley: Working with FA support on known issues (login disconnect, pdf text overlap), Discussing requirements for new form "appropriateness assessment"</li><li>EMIR/SFTR: Creating new fields and record types on Web Form for the process, Setting up mapping and connector FA → Salesforce for CY form</li><li>MaxComply finalizing back integration tests</li><li>Conga Composer - finalizing fixes in SELT registration forms</li><li>Calypso integration  - providing requirements to ESB for the final version of integration (including target data structure for EMIR/SFTR)</li></ul>FO<ul><li>Разбирались с проблемой не загруженных сделок совершенных в выходные дни. В новой версии приложения нам не удалось воспроизвести ситуацию, когда часть сделок теряется при отправке в НТ. В целом в сервисе не очень хорошо реализован учет уже загруженных сделок, видим в этом потенциальную возможность повторения проблемы. Для гарантированного исправления требуется рефакторинг сервиса. Решение проблемы с редактирование Manual Trades [http://jira/browse/FOIT-85](http://jira/browse/FOIT-85), устранили баг, ждем согласования на вывод в прод. Разработка в рамках задачи QUIK БКС Брокер - работа в выходные дни ([http://jira/browse/REQ-1339](http://jira/browse/REQ-1339)) Анализ по задаче Dynamic Report ([http://jira/browse/REQ-1476](http://jira/browse/REQ-1476))</li></ul> | 
| top 3-5 points | 
| 
1. Нужно обсудить кто что делает и отвечает за процесс подготовки архитектур. Я на этой неделе сделал CPORT архитектуру, но она получила 100500 критик и замечаний. напрашивается, чтобы их делал Макс и отвечал за них. Аналогично в пайпе арх по EDW, Kondor.
1. Прилетела сверх неожиданно задача по новым форматам файлов SFTR, поставили всех на уши. В итоге Леша В. в выходные выходит спеку писать, Рому переаллоцировали из FX на эту задачу на след неделе
1.  **!!!!**  Леша Варфоломеев сказал, что отправили последние файлы по бэк репортингу. Последние ответы в пятницу еще не получили. ВАЖНО!!! Нужно обязательно чтобы было письмо на всю тусовку, что задача выполнена и отблагодарить всех и в частности Лешу Варфоломеева. Ему бы оч хотелось, чтобы это было отмечено. У нас очень мало позитива!!
1. Проблема с тормозами с пост-трейд репортинг на Кондор получила неожиданный поворот - очень медленная скорость записи на диск в Базу из сервера где квик экспортер, с локала быстро. Теперь выход Макса, но мне непонятно где и что смотреть
1. Актуализиурем бюджет по проекту Систематики Лимит-сервера. Я промахнулся с бюджетом при расчете - не учли оценку стоек в ДЦ. Отдельно обсудим

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
| Kondor
1. Продолжаем совместно с другими командами работать над проблемой экспортеров. 
1. В этом релизе запланирован вывод последней задачи на стороне К+ проекта NT-Pro.
1. Была проведена ознакомительная встреча с обновленной Казной. Познакомились. Далее будем координировать в рабочем порядке. Про проект перевода фондирования, который ведет Рохлина, они знают.
1. Вывели в прод одну из задач OPS Efficiency по сверкам - репо. "-й день, полет нормальный.

CPORT
1. Задачи по ресерч порталу - улучшение работы фильтров, добавление новых
1. Отчитались о результатах спринта коллегам из ресерч

EDW<ul><li>SCS. Add filter into ssi reference rules on field country_id</li><li>SCS. E-Disclosure notification</li><li>Portfolio reconciliation</li><li>SFTR Reconciliation in Reg Reporting Service</li><li>FX Option</li></ul>CRM<ul><li>Pre-analysis for Digital Communications Channels Project</li><li>FormAssembley: Working with FA support on known issues (login disconnect, pdf text overlap), Discussing requirements for new form "appropriateness assessment"</li><li>EMIR/SFTR: Creating new fields and record types on Web Form for the process, Setting up mapping and connector FA → Salesforce for CY form</li><li>MaxComply finalizing back integration tests</li><li>Conga Composer - finalizing fixes in SELT registration forms</li><li>Calypso integration  - providing requirements to ESB for the final version of integration (including target data structure for EMIR/SFTR)</li></ul>FO<ul><li>Разбирались с проблемой не загруженных сделок совершенных в выходные дни. В новой версии приложения нам не удалось воспроизвести ситуацию, когда часть сделок теряется при отправке в НТ. В целом в сервисе не очень хорошо реализован учет уже загруженных сделок, видим в этом потенциальную возможность повторения проблемы. Для гарантированного исправления требуется рефакторинг сервиса. Решение проблемы с редактирование Manual Trades [http://jira/browse/FOIT-85](http://jira/browse/FOIT-85), устранили баг, ждем согласования на вывод в прод. Разработка в рамках задачи QUIK БКС Брокер - работа в выходные дни ([http://jira/browse/REQ-1339](http://jira/browse/REQ-1339)) Анализ по задаче Dynamic Report ([http://jira/browse/REQ-1476](http://jira/browse/REQ-1476))</li></ul> | 
| top 3-5 points | 
| 
1. Нужно обсудить кто что делает и отвечает за процесс подготовки архитектур. Я на этой неделе сделал CPORT архитектуру, но она получила 100500 критик и замечаний. напрашивается, чтобы их делал Макс и отвечал за них. Аналогично в пайпе арх по EDW, Kondor.
1. Прилетела сверх неожиданно задача по новым форматам файлов SFTR, поставили всех на уши. В итоге Леша В. в выходные выходит спеку писать, Рому переаллоцировали из FX на эту задачу на след неделе
1.  **!!!!**  Леша Варфоломеев сказал, что отправили последние файлы по бэк репортингу. Последние ответы в пятницу еще не получили. ВАЖНО!!! Нужно обязательно чтобы было письмо на всю тусовку, что задача выполнена и отблагодарить всех и в частности Лешу Варфоломеева. Ему бы оч хотелось, чтобы это было отмечено. У нас очень мало позитива!!
1. Проблема с тормозами с пост-трейд репортинг на Кондор получила неожиданный поворот - очень медленная скорость записи на диск в Базу из сервера где квик экспортер, с локала быстро. Теперь выход Макса, но мне непонятно где и что смотреть
1. Актуализиурем бюджет по проекту Систематики Лимит-сервера. Я промахнулся с бюджетом при расчете - не учли оценку стоек в ДЦ. Отдельно обсудим

 | 







*****

[[category.storage-team]] 
[[category.confluence]] 
