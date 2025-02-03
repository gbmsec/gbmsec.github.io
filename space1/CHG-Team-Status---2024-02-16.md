





| CHG

 | 
| Alexey Dorogov

 | 
| 

 | 
| CRM

1) Salesforce UK:

<ul><li>First succesful week of SF UK exploitation: fixing minor errors, extra support for users</li><li> AML Risk Level Review process released for SF UK</li></ul>2) EMIR-Refit - Initial analysis with O.Dudolina

3) Проект "К" - Первичное обсуждение требований к Кипру как к QI в части хранения налоговой информации клиентов и их налоговых ставок, и проистекающие из этого доработки

4) Service Cloud

<ul><li>Согласование формата закупки</li><li>Запрос документов у вендора</li></ul>

Calypso:

<ul><li>Работали над приоритетными SR'ами и исправлением багов. </li><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - проводим тестирование текущего функционала в 17 версии</li><li>BCSGL - проводим тестирование текущего функционала в 17 версии. Поставили задачи на ESB для преобразования внешних выписок для сверок в Calypso.</li><li>BCSUK - исследовали функционал по фандированию. Изучили алгоритм попадания сделок.</li><li>Провели первую встречу с аудиторами CUSIP по поводу загрузки данных из Bloomberg. </li><li>Тестируем развернутые новые инстансы Calypso 17 на Кипре PREPCY17 и UATCY17. Протестировали интеграции - успешно. Ручные изменения статики - успешно. Ожидаем тестирования букирования сделок с Казахстаном и тестирование TSL.</li></ul>IBQ: Продолжаем делать аналитику и разработку по проекту EMIR Refit. 



Riskroom:

<ul><li>ArmRm - testing and test results discussion</li><li>qkCurrencyRate function replacement for UK - testing in progress</li><li>Working on CMA room enhancements for CDS portfolio calc for Emir/refit - sent test message to EDW ok</li></ul>FX:

<ul><li>Weekendrates service - fixed a bug updating markups. UAT</li><li>DB SQL timeout problem arises at NtPro, need to migrate to another server -  planned on 24/02, to plan</li><li>Banded tariffication to be tested</li><li>Started to implement Unusual client activity alarm</li><li>DynRep discussed</li></ul>OneTick, SFTR: - SL3 issues

EMIR/REFIT: RR related task (CMA room) - implementation started on EDW side



EDW

<ul><li>KT from Alexander Kravchenko</li><li>1 interview</li></ul>

Кондор


1.  **Ресурсная проблема отсутствия разработчика создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Получили от Систематики первую версию ТЗ.
1. В этом релизе обновляем версию Модулляра.
1. На нас вышли  с возможностью обработки в К+ решение по Product Governance. Комплаенс Кипра (Нателла) проговорила, что может выйти на рук-во ИТ с приоритезацией данной задачи по отношению к проекту перехода на Атриум.



 | 
| top 3-5 points | 
| 1) ISIN коды американских бумаг на ЮКБыл звонок на ЮК с аудитором. Надо обсудить. Есть информация как это проходило и что спрашивают. И в связи с имеющейся инфой надо понять что делаем по теме Кипра.2) Тендер на ресурсы в Группе3) Сложности с поиском и подбором. Сейчас ищем по шине, от других я вообще ничего не вижу, никакой активности4) Qort и проблема производительностиНеобходимо на общей встрече еще раз проговорить известную проблему с Кортом и Кипром, чтобы руководители довели до сотрудников. Мы знаем, что периодически возникает проблема, что Корт утром запускает очень долго. Это происходит по причине того, что при изменении таблицы активов приходится ее скачивать полностью всем пользователям, кто запускает систему. Объем закачки - 200 МБ. Это может занимать 20 минут или более из-за того, что канал до Кипра обладает существенным ограничением производительности. На эту особенность завели Проблему с типом known Issue | 
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

1) Salesforce UK:

<ul><li>First succesful week of SF UK exploitation: fixing minor errors, extra support for users</li><li> AML Risk Level Review process released for SF UK</li></ul>2) EMIR-Refit - Initial analysis with O.Dudolina

3) Проект "К" - Первичное обсуждение требований к Кипру как к QI в части хранения налоговой информации клиентов и их налоговых ставок, и проистекающие из этого доработки

4) Service Cloud

<ul><li>Согласование формата закупки</li><li>Запрос документов у вендора</li></ul>

Calypso:

<ul><li>Работали над приоритетными SR'ами и исправлением багов. </li><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - проводим тестирование текущего функционала в 17 версии</li><li>BCSGL - проводим тестирование текущего функционала в 17 версии. Поставили задачи на ESB для преобразования внешних выписок для сверок в Calypso.</li><li>BCSUK - исследовали функционал по фандированию. Изучили алгоритм попадания сделок.</li><li>Провели первую встречу с аудиторами CUSIP по поводу загрузки данных из Bloomberg. </li><li>Тестируем развернутые новые инстансы Calypso 17 на Кипре PREPCY17 и UATCY17. Протестировали интеграции - успешно. Ручные изменения статики - успешно. Ожидаем тестирования букирования сделок с Казахстаном и тестирование TSL.</li></ul>IBQ: Продолжаем делать аналитику и разработку по проекту EMIR Refit. 



Riskroom:

<ul><li>ArmRm - testing and test results discussion</li><li>qkCurrencyRate function replacement for UK - testing in progress</li><li>Working on CMA room enhancements for CDS portfolio calc for Emir/refit - sent test message to EDW ok</li></ul>FX:

<ul><li>Weekendrates service - fixed a bug updating markups. UAT</li><li>DB SQL timeout problem arises at NtPro, need to migrate to another server -  planned on 24/02, to plan</li><li>Banded tariffication to be tested</li><li>Started to implement Unusual client activity alarm</li><li>DynRep discussed</li></ul>OneTick, SFTR: - SL3 issues

EMIR/REFIT: RR related task (CMA room) - implementation started on EDW side



EDW

<ul><li>KT from Alexander Kravchenko</li><li>1 interview</li></ul>

Кондор


1.  **Ресурсная проблема отсутствия разработчика создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Получили от Систематики первую версию ТЗ.
1. В этом релизе обновляем версию Модулляра.
1. На нас вышли  с возможностью обработки в К+ решение по Product Governance. Комплаенс Кипра (Нателла) проговорила, что может выйти на рук-во ИТ с приоритезацией данной задачи по отношению к проекту перехода на Атриум.



 | 
| top 3-5 points | 
| 1) ISIN коды американских бумаг на ЮКБыл звонок на ЮК с аудитором. Надо обсудить. Есть информация как это проходило и что спрашивают. И в связи с имеющейся инфой надо понять что делаем по теме Кипра.2) Тендер на ресурсы в Группе3) Сложности с поиском и подбором. Сейчас ищем по шине, от других я вообще ничего не вижу, никакой активности4) Qort и проблема производительностиНеобходимо на общей встрече еще раз проговорить известную проблему с Кортом и Кипром, чтобы руководители довели до сотрудников. Мы знаем, что периодически возникает проблема, что Корт утром запускает очень долго. Это происходит по причине того, что при изменении таблицы активов приходится ее скачивать полностью всем пользователям, кто запускает систему. Объем закачки - 200 МБ. Это может занимать 20 минут или более из-за того, что канал до Кипра обладает существенным ограничением производительности. На эту особенность завели Проблему с типом known Issue | 







*****

[[category.storage-team]] 
[[category.confluence]] 
