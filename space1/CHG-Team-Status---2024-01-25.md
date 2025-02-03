





| CHG

 | 
| Alexey 

 | 
| 

 | 
| PRJ-310 Emir Refit [http://jira/secure/StructureBoard.jspa?s=140#](http://jira/secure/StructureBoard.jspa?s=140)



Calypso:

<ul><li>BCSCY - Сделали и с релизом выводим OTC Agency Repo. Отдали в тест Lequidity Report. Занимаемся анализом доработок по брокерскому отчету.</li><li>BCSGL - доделали багфиксинг по TSL к релизу.</li><li>BCSUK - пофиксили баг с отображением статусов сетелмента на трасфере. Провели демонстрацию букирования сделок в Калипсо для пользователей UK - bcp решение.</li><li>CASS - поправили ошибки, которые были найдены на CY. </li><li>Тестируем локально развернутый новый инстанс Calypso 17 на NV ресурсом QA. Делаем задачу по исправлению кода, то что нашел Алексей Сидоркин в ходе предварительного анализа.</li><li>Провели планирование задач на новый релиз.</li></ul>IBQ:

<ul><li>Продолжаем делать аналитику по проекту EMIR Refit. Делаем разработку по обработке событий + новый отчет по Margin Report.</li><li>Сделали 4 срочных SR по IBQ, а также хотим обновить логику формирования данных в сервисе FIRDS, чтобы публиковать списки репортабл инструментов в Calypso PRODCY и EDW EP.</li><li>Вместе с командой RiskRoom пытаемся определиться с параметрами сделок из QORT на автоматическую загрузку в RiskRoom</li><li>Новый аналитик на аутсорс, делает выгрузки данных по OT и занимается задачей по загрузке данных из Anna DSB в EDW для EMIR Refit проекта.</li></ul>CRM1) Migration of UK CRM service<ul><li>data migration complete</li><li>files migration complete</li><li>Развёрнута тестовой среда типа Partial Copy (с копией части записей дб)</li><li>IT internal testing started</li></ul>2) Оплата счёта FormAssembly на KZ<ul><li>счёт полностью согласован и ждёт оплаты</li><li>вендор скоординирован по ожиданию просроченного платежа без отключения сервиса</li></ul>3) Восстановление функционала Conga Composer для риск менеджмента группы на SF Non-UK (отправка отчетов в АРМ РМ через файлы по почте)4) Service Cloud - обсуждение вариантов сетапа, а также тайминга закупкиEDW<ul><li>Uploading agreement</li><li>Uploading conf date</li><li>Deligated Reporting Flag MRRA</li><li>Bug Fixing</li></ul>Riskroom:<ul><li>Moved EP emails to ep EWS/smtp</li><li>ArmRm - moving forward with an intraday report</li><li>qkCurrencyRate function replacement for UK is ready, to test next week</li></ul>FX:<ul><li>DB SQL timeout problem arises at NtPro and MD databases, fix for WeekendRates so it does not stops delivered to UAT</li><li>Banded tariffication testing started and stopped again at bank side</li><li>Started to implement Unusual client activity alarm</li></ul>OneTick:<ul><li>AIX and other changes deployed to UAT</li></ul>EMIR/REFIT:<ul><li>One more task when to dev (Margin report)</li><li>RR related task (CMA room) - pre-analysis started</li><li>Possibility to add csv export functionality is being investigated</li></ul>RegReporting<ul><li>Continued fixing SC reconciliation service at UK</li><li>None RegT reconciliation service is working properly, and no user demand so far, to investigate further</li><li>Preparing architecture diagram</li></ul>Kondor
1.  **Ресурсная проблема создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Систематика предоставила план с датами выхода || run шлюза в мае.
1. Проведены консультации по возможности outsource компании TRM (Иван Лисенков). Рассматриваем возможность заключения с ними рамочного договора.
1. Проведена встреча по итогам инцидентов по репортингу прошлой недели. Принято решение по алертингу пойманных кейсов. Репортинг team-у передан дашборд графаны по  мониторингу отправки сообщений в TradeEcho.
1. Есть кандидат(ка), что в принципе подходит на аналитика. При прочих равных (отрицательное решение по Крутину и Яшину, а также если не удастся опыт поиска по Локатору) - можно брать. Опыт ИБ бизнеса, правда , со стороны Диасофта.

 | 
| top 3-5 points | 
| 1)  **Электронный каналы коммуникаций внутри** .

Есть что обсудит: Канал с публикацией новостей, канал для оповещений по процедурам. 

Как раз обсуждали про Тимз и Жиру, но нам нужно немного другое. В частности по аудиту Кипра есть такие вопросы



2) ОХД - ситуация с ресурсами. Ниже ситуация с ресурсами всех ОХД команды, это не то что на ИБ аллоцировано, а всего

Dev - 2 разработчика, 2 вакансии

An - 2 аналитика, 1 вакансия.

Сообщили, что как куратором будет Федоров Александр из КХД, но еще с ним не говорили.

Ресурсов оч мало в сравнении с теми активностями, что заявлено.



3) Ситуация с допником на ВДКом - не могут подписать, опять "какие то проблемы".  4) По поиску и заполнения вакансий на шину. Все оч грустно. Все что были на рассмотрении все отвалились. Ищем с Апреля. Скоро будет год этой активности.

5) HR5.1) Нас покидает Саша Кравченко. До этого ушел Коля. Уходит больше чем приходит, значительно.5.2.) Подсвечиваю ключевых сотрудников, еще раз, кого некем заменять - Саша А., Денис Р., Саша Корнилов., Команда К (там почти пусто), Костя, Илья, Антон, Юля Л., Олег Е., Оля Арс. У нас уже большинство людей перешло в разряд критичных - т.к. они долгое время в единственном числе  и на них критичные функции. | 
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
| PRJ-310 Emir Refit [http://jira/secure/StructureBoard.jspa?s=140#](http://jira/secure/StructureBoard.jspa?s=140)



Calypso:

<ul><li>BCSCY - Сделали и с релизом выводим OTC Agency Repo. Отдали в тест Lequidity Report. Занимаемся анализом доработок по брокерскому отчету.</li><li>BCSGL - доделали багфиксинг по TSL к релизу.</li><li>BCSUK - пофиксили баг с отображением статусов сетелмента на трасфере. Провели демонстрацию букирования сделок в Калипсо для пользователей UK - bcp решение.</li><li>CASS - поправили ошибки, которые были найдены на CY. </li><li>Тестируем локально развернутый новый инстанс Calypso 17 на NV ресурсом QA. Делаем задачу по исправлению кода, то что нашел Алексей Сидоркин в ходе предварительного анализа.</li><li>Провели планирование задач на новый релиз.</li></ul>IBQ:

<ul><li>Продолжаем делать аналитику по проекту EMIR Refit. Делаем разработку по обработке событий + новый отчет по Margin Report.</li><li>Сделали 4 срочных SR по IBQ, а также хотим обновить логику формирования данных в сервисе FIRDS, чтобы публиковать списки репортабл инструментов в Calypso PRODCY и EDW EP.</li><li>Вместе с командой RiskRoom пытаемся определиться с параметрами сделок из QORT на автоматическую загрузку в RiskRoom</li><li>Новый аналитик на аутсорс, делает выгрузки данных по OT и занимается задачей по загрузке данных из Anna DSB в EDW для EMIR Refit проекта.</li></ul>CRM1) Migration of UK CRM service<ul><li>data migration complete</li><li>files migration complete</li><li>Развёрнута тестовой среда типа Partial Copy (с копией части записей дб)</li><li>IT internal testing started</li></ul>2) Оплата счёта FormAssembly на KZ<ul><li>счёт полностью согласован и ждёт оплаты</li><li>вендор скоординирован по ожиданию просроченного платежа без отключения сервиса</li></ul>3) Восстановление функционала Conga Composer для риск менеджмента группы на SF Non-UK (отправка отчетов в АРМ РМ через файлы по почте)4) Service Cloud - обсуждение вариантов сетапа, а также тайминга закупкиEDW<ul><li>Uploading agreement</li><li>Uploading conf date</li><li>Deligated Reporting Flag MRRA</li><li>Bug Fixing</li></ul>Riskroom:<ul><li>Moved EP emails to ep EWS/smtp</li><li>ArmRm - moving forward with an intraday report</li><li>qkCurrencyRate function replacement for UK is ready, to test next week</li></ul>FX:<ul><li>DB SQL timeout problem arises at NtPro and MD databases, fix for WeekendRates so it does not stops delivered to UAT</li><li>Banded tariffication testing started and stopped again at bank side</li><li>Started to implement Unusual client activity alarm</li></ul>OneTick:<ul><li>AIX and other changes deployed to UAT</li></ul>EMIR/REFIT:<ul><li>One more task when to dev (Margin report)</li><li>RR related task (CMA room) - pre-analysis started</li><li>Possibility to add csv export functionality is being investigated</li></ul>RegReporting<ul><li>Continued fixing SC reconciliation service at UK</li><li>None RegT reconciliation service is working properly, and no user demand so far, to investigate further</li><li>Preparing architecture diagram</li></ul>Kondor
1.  **Ресурсная проблема создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Систематика предоставила план с датами выхода || run шлюза в мае.
1. Проведены консультации по возможности outsource компании TRM (Иван Лисенков). Рассматриваем возможность заключения с ними рамочного договора.
1. Проведена встреча по итогам инцидентов по репортингу прошлой недели. Принято решение по алертингу пойманных кейсов. Репортинг team-у передан дашборд графаны по  мониторингу отправки сообщений в TradeEcho.
1. Есть кандидат(ка), что в принципе подходит на аналитика. При прочих равных (отрицательное решение по Крутину и Яшину, а также если не удастся опыт поиска по Локатору) - можно брать. Опыт ИБ бизнеса, правда , со стороны Диасофта.

 | 
| top 3-5 points | 
| 1)  **Электронный каналы коммуникаций внутри** .

Есть что обсудит: Канал с публикацией новостей, канал для оповещений по процедурам. 

Как раз обсуждали про Тимз и Жиру, но нам нужно немного другое. В частности по аудиту Кипра есть такие вопросы



2) ОХД - ситуация с ресурсами. Ниже ситуация с ресурсами всех ОХД команды, это не то что на ИБ аллоцировано, а всего

Dev - 2 разработчика, 2 вакансии

An - 2 аналитика, 1 вакансия.

Сообщили, что как куратором будет Федоров Александр из КХД, но еще с ним не говорили.

Ресурсов оч мало в сравнении с теми активностями, что заявлено.



3) Ситуация с допником на ВДКом - не могут подписать, опять "какие то проблемы".  4) По поиску и заполнения вакансий на шину. Все оч грустно. Все что были на рассмотрении все отвалились. Ищем с Апреля. Скоро будет год этой активности.

5) HR5.1) Нас покидает Саша Кравченко. До этого ушел Коля. Уходит больше чем приходит, значительно.5.2.) Подсвечиваю ключевых сотрудников, еще раз, кого некем заменять - Саша А., Денис Р., Саша Корнилов., Команда К (там почти пусто), Костя, Илья, Антон, Юля Л., Олег Е., Оля Арс. У нас уже большинство людей перешло в разряд критичных - т.к. они долгое время в единственном числе  и на них критичные функции. | 







*****

[[category.storage-team]] 
[[category.confluence]] 
