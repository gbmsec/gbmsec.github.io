





| CHG

 | 
| Alexey 

 | 
| 

 | 
| Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - Тестируем и дорабатываем MiFID репорт. Передали в UAT Liquidity Report. Начали разработку CA по CASS сделкам. Протестировали загрузку CDS сделок из файла. CFD - делаем загрузку сделок через FIX.</li><li>BCSGL - сделали мелкий багфиксинг по TSL. Настраиваем подключение к QUIK экспортеру.</li><li>BCSUK - поставили критичную доработку по MiFID Post Trade Reporting, связанную с изменением требований законодательства. Тестируем переключение загрузки карточек КД с Markit на Euroclear</li></ul>IBQ:

<ul><li>Проводим UAT по проекту EMIR Refit + багфиксинг. </li><li>Сделали несколько критичных SR и багов по IBQ</li><li>Сформировали квартальную отчетность по Кипру.</li></ul>

Riskroom:

<ul><li>continue to analyze and implement tasks related to decommission of Qort</li><li>new task "Limits to MM" was initially discussed, waiting for SR and reqs - still in progress - cancelled</li><li>moving Quik autolimits functionality to EP - in progress</li><li>ARM RM limits - new enhancements were delivered, waiting for feedback</li></ul>FX:

<ul><li>Unusual client activity added to UI: UAT</li><li>Some minor fixes for adding new pairs, etc.</li><li>DynRep: stopping development until 1 view is ready at IBSO side</li><li>Task to analyze productivity of Unusual activities monitor is done, 10sec is reasonable minimum</li></ul>OneTick, SFTR, Regreporting:

<ul><li>SFTR change for SFTR questionnarie is at UAT, waiting for test results</li><li>OneTick: implementation for marex - UAT, new reqs implemented, what's next?</li><li>Discussions on reporting service approach, Draft demo was discussed with AVyugovskiy</li></ul>EMIR/REFIT:

<ul><li>Prepare for release and support</li></ul>EDW

<ul><li>Prepare for Emir-Refit release:<ul><li>EDW</li><li>AnnaDSB loader service</li><li>Firds-EDW loader service</li></ul></li><li>new SR (SFTR qustionnarie) development is done, testing</li><li>to stop NSD services at UK (not done)</li></ul>Атриум-Кондор
1. Новый разработчик - получил все, пока нужные, доступы, приступил к изучению материала.
1. Систематика приступила к отладке || run шлюза (в своей тестовой среде) на наших прод данных.
1. Установка ПО Атриума в прод среде должна быть проведена непосредственно перед запуском (Систематика).
1. Разработано решение по загрузке фин инструментов из Калипсо в Атриум. 
1. Начался проект Product Governance. Нежелательно делать в К+, чтобы потом переделывать в Атриуме. 

 | 
| top 3-5 points | 
| Оплатили ВДКом за февраль и март.Осталось подписать ТЗ на апрель-июньOpenTRM (Кондор) - в процессе согласования подрядчика все еще.В период 29-1 мая будет запуск отчетности по новым правилам. Будем много проблем, как нам кажется.!!! По коллективу отмечены большие ожидания в части информации по бонусам и переоценке. Я получил огромное число вопросов на это неделе.!!! Будем выводить функционал по Рефиту. Костя ожидает много рпороблем и что гладко деплой не пройдет. Много всего надо на ЕДВ ставить, а опыта пока мало, т.к. Саши больше нет. В общем без проблем для нас это не пройдетДобей плз тему с согласование оплаты по работам в майские по РефитуНе можем согласовать внутри ИТ как будут устанавливаться сервера Систематики. Мое мнение - для установки можно пустить на них вендора, потом доступ отобрать. Возражает Максим Васильев. | 
|  --- | 
|  --- | 
|  --- | 
|  --- | 
|  --- | 
|  --- | 
| CHG

 | 
| Alexey 

 | 
| 

 | 
| Calypso:

<ul><li>Из проектов работаем над задачами:<ul><li>Setup BCSCY in Calypso Non UK</li><li>K Project</li><li>Marex BCSGL Project</li></ul></li></ul><ul><li>BCSCY - Тестируем и дорабатываем MiFID репорт. Передали в UAT Liquidity Report. Начали разработку CA по CASS сделкам. Протестировали загрузку CDS сделок из файла. CFD - делаем загрузку сделок через FIX.</li><li>BCSGL - сделали мелкий багфиксинг по TSL. Настраиваем подключение к QUIK экспортеру.</li><li>BCSUK - поставили критичную доработку по MiFID Post Trade Reporting, связанную с изменением требований законодательства. Тестируем переключение загрузки карточек КД с Markit на Euroclear</li></ul>IBQ:

<ul><li>Проводим UAT по проекту EMIR Refit + багфиксинг. </li><li>Сделали несколько критичных SR и багов по IBQ</li><li>Сформировали квартальную отчетность по Кипру.</li></ul>

Riskroom:

<ul><li>continue to analyze and implement tasks related to decommission of Qort</li><li>new task "Limits to MM" was initially discussed, waiting for SR and reqs - still in progress - cancelled</li><li>moving Quik autolimits functionality to EP - in progress</li><li>ARM RM limits - new enhancements were delivered, waiting for feedback</li></ul>FX:

<ul><li>Unusual client activity added to UI: UAT</li><li>Some minor fixes for adding new pairs, etc.</li><li>DynRep: stopping development until 1 view is ready at IBSO side</li><li>Task to analyze productivity of Unusual activities monitor is done, 10sec is reasonable minimum</li></ul>OneTick, SFTR, Regreporting:

<ul><li>SFTR change for SFTR questionnarie is at UAT, waiting for test results</li><li>OneTick: implementation for marex - UAT, new reqs implemented, what's next?</li><li>Discussions on reporting service approach, Draft demo was discussed with AVyugovskiy</li></ul>EMIR/REFIT:

<ul><li>Prepare for release and support</li></ul>EDW

<ul><li>Prepare for Emir-Refit release:<ul><li>EDW</li><li>AnnaDSB loader service</li><li>Firds-EDW loader service</li></ul></li><li>new SR (SFTR qustionnarie) development is done, testing</li><li>to stop NSD services at UK (not done)</li></ul>Атриум-Кондор
1. Новый разработчик - получил все, пока нужные, доступы, приступил к изучению материала.
1. Систематика приступила к отладке || run шлюза (в своей тестовой среде) на наших прод данных.
1. Установка ПО Атриума в прод среде должна быть проведена непосредственно перед запуском (Систематика).
1. Разработано решение по загрузке фин инструментов из Калипсо в Атриум. 
1. Начался проект Product Governance. Нежелательно делать в К+, чтобы потом переделывать в Атриуме. 

 | 
| top 3-5 points | 
| Оплатили ВДКом за февраль и март.Осталось подписать ТЗ на апрель-июньOpenTRM (Кондор) - в процессе согласования подрядчика все еще.В период 29-1 мая будет запуск отчетности по новым правилам. Будем много проблем, как нам кажется.!!! По коллективу отмечены большие ожидания в части информации по бонусам и переоценке. Я получил огромное число вопросов на это неделе.!!! Будем выводить функционал по Рефиту. Костя ожидает много рпороблем и что гладко деплой не пройдет. Много всего надо на ЕДВ ставить, а опыта пока мало, т.к. Саши больше нет. В общем без проблем для нас это не пройдетДобей плз тему с согласование оплаты по работам в майские по РефитуНе можем согласовать внутри ИТ как будут устанавливаться сервера Систематики. Мое мнение - для установки можно пустить на них вендора, потом доступ отобрать. Возражает Максим Васильев. | 







*****

[[category.storage-team]] 
[[category.confluence]] 
