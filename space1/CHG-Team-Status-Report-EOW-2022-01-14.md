





| CHG

 | 
| Alexey Dorogov

 | 
|  

 | 
| EDW

<ul><li>Analysis SFTR bugs</li><li>Fix uploading entity delegated reporting from SF</li><li>SCS. Implement integratin sanction list. New format</li><li>SCS. Implement new BBG sanction mapping</li><li>Upload OTC Internal SLB into EDW</li><li>Portfolio reconciliation</li><li>SFTR Reconciliation in Reg Reporting Service</li></ul>Kondor


1. Словили инцидент, связанный с включением Sybase audit для аудита. Причина - некорректная настройка функционала.
1. Проводилось тестирование чистки избыточных данных в таблицах. Результаты подлежат анализу.
1. Подготовлен релиз с задачами по переводу Дельты на UK - первые сделки планируются 17.01.
1. Получено устное согласие Систематики начать работать по 15-минутной отчетности на МБ по гарантийному письму. Пытаюсь добиться письменного ответа, но Курочкин болеет...

IBQ:

<ul><li>Провели планирование задач на новый спринт.</li><li>Из-за изменения настроек безопасности на стороне FCA, у нас перестали загружаться файлы с репортабл инструментами. Решили вынести этот функционал в отдельный микросервис. Активно ведется разработка. Планируем на следующей неделе вывести его в PROD.</li><li>Вывели релиз</li></ul>CPORT
1. Тестирование сервиса калипсо в бизнес процессе
1. Поменяли логику сохранения настроек нотификаций для ресерч
1. Починили баг с загрузкой инструментов на портал

FO
1. [FOIT-75](http://jira/browse/FOIT-75) Quotes validation for weekend FX rates - выведено в UAT
1. Настроили логирование курсов из таблицы \[MD].\[dbo].\[ClientRate]
1. [FOIT-76](http://jira/browse/FOIT-76) - разработка документации для FX Rates сервисов
1. Вывели в тест функционал по задачам [FOIT-79](http://jira/browse/FOIT-79) и [FOIT-80](http://jira/browse/FOIT-80) (Очистка буфера и уменьшение объема логов сервиса)

 | 
| top 3-5 points | 
| FX teams wants 24/7 FX quotation - мы к этому не готовы по многим причинам | 
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

<ul><li>Analysis SFTR bugs</li><li>Fix uploading entity delegated reporting from SF</li><li>SCS. Implement integratin sanction list. New format</li><li>SCS. Implement new BBG sanction mapping</li><li>Upload OTC Internal SLB into EDW</li><li>Portfolio reconciliation</li><li>SFTR Reconciliation in Reg Reporting Service</li></ul>Kondor


1. Словили инцидент, связанный с включением Sybase audit для аудита. Причина - некорректная настройка функционала.
1. Проводилось тестирование чистки избыточных данных в таблицах. Результаты подлежат анализу.
1. Подготовлен релиз с задачами по переводу Дельты на UK - первые сделки планируются 17.01.
1. Получено устное согласие Систематики начать работать по 15-минутной отчетности на МБ по гарантийному письму. Пытаюсь добиться письменного ответа, но Курочкин болеет...

IBQ:

<ul><li>Провели планирование задач на новый спринт.</li><li>Из-за изменения настроек безопасности на стороне FCA, у нас перестали загружаться файлы с репортабл инструментами. Решили вынести этот функционал в отдельный микросервис. Активно ведется разработка. Планируем на следующей неделе вывести его в PROD.</li><li>Вывели релиз</li></ul>CPORT
1. Тестирование сервиса калипсо в бизнес процессе
1. Поменяли логику сохранения настроек нотификаций для ресерч
1. Починили баг с загрузкой инструментов на портал

FO
1. [FOIT-75](http://jira/browse/FOIT-75) Quotes validation for weekend FX rates - выведено в UAT
1. Настроили логирование курсов из таблицы \[MD].\[dbo].\[ClientRate]
1. [FOIT-76](http://jira/browse/FOIT-76) - разработка документации для FX Rates сервисов
1. Вывели в тест функционал по задачам [FOIT-79](http://jira/browse/FOIT-79) и [FOIT-80](http://jira/browse/FOIT-80) (Очистка буфера и уменьшение объема логов сервиса)

 | 
| top 3-5 points | 
| FX teams wants 24/7 FX quotation - мы к этому не готовы по многим причинам | 







*****

[[category.storage-team]] 
[[category.confluence]] 
