





| CHG

 | 
| Alexey

 | 
| 

 | 
| Calypso:<ul><li>BCSCY - продолжаем процесс UAT по Trade / Netting Confirmation. Тестировали смену роли с Custody на CASS client со всеми downstream системами. Делаем аналитику по Liquidity Management Report. Начали тестирование MiFID Transaction репорт в рамках проекта по миграции Кипра. Досетапили продукт CDS для Кипра.</li></ul><ul><li>BCSGL - дали свои оценки по сетапу продукта FX Spot. Сделали багфиксинг и хотфикс по TSL.</li><li>BCSUK - поправили статику для корректного рассчета Accruel Interest по сделкам. По FX разобрали как считается поле TradePrice.</li><li>CASS - исправили в UK ошибки в Position Keeper и Inventory Report по запросам деска UK.</li><li>Тестируем локально развернутый новый инстанс Calypso 17 на NV ресурсом QA. Делаем задачу по исправлению кода, то что нашел Алексей Сидоркин в ходе предварительного анализа.</li></ul>IBQ:<ul><li>Продолжаем делать аналитику по проекту EMIR Refit. Делаем разработку по обработке событий + аналитику по Margin Report.</li><li>Вместе с командой RiskRoom пытаемся определиться с параметрами, которые должны рассчитываться для MarginReport EMIR Refit.</li><li>Новый аналитик на аутсорс, начал заниматься задачей по загрузке данных из Anna DSB в EDW для EMIR Refit проекта.</li><li>Занимались восстановлением тестовой среды QORT, чтобы запустить процесс UAT по задачам релиза.</li></ul>Кондор
1.  **Ресурсная проблема создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Для ИТ руководства обозначены критичные риски проекта перехода на Атриум
1. Проведена встреча с А. Курочкиным (руководитель Систематики) на уровне нашего ИТ руководства. Обозначена наша цель запуститься с || run gateway в мае.
1. !!! Выявлен gap ресурса ИТ ИБ команды БО (Корт) на поддержку проекта перехода на Атриум.

Riskroom:<ul><li>ArmRm - more calrification came to continue ArmRm project</li><li>Email service to implement EWS at EP is ready to go live</li></ul>FX:<ul><li>Dev continues for banded tariffication, delployed to UAT, procedural API for bank agreed, testing stopped at bank side</li><li>New WeekendRates service deployed to UAT</li><li>EWS task: services are being analyzed whether they have email functionality</li></ul>OneTick: Ready to deploy latest changes to EPEMIR/REFIT:<ul><li>More reqs needed</li><li>RR related task (CMA room) - pre-analysis started</li></ul>RegReporting<ul><li>Sorted out major mess at UK, also at UAT</li><li>Continue fixing SC reconciliation service at UK</li><li>None RegT reconciliation service is working properly, and no user demand so far, to investigate further</li><li>Preparing architecture diagram</li></ul>CRM1) Migration of UK CRM service<ul><li>Migration of metadata complete</li><li>Start of data migration</li><li>Preparation for files migration</li><li>Full backup of old data (in case there is no prolongation) </li><li>Switch off letter for old Salesforce org signed and process is started.</li></ul>2) Full CY clientbase upload & support in CRM - providing colleagues with the list of required data with format and comments 3) Обновление справочника ЦФО 2024 - маппинг текущих значений на новые4) Процессинг счета на FormAssembly KZ<ul><li>попытки протолкнуть и найти финансирование в  бюджете</li><li>огранизация встречи с вендором на тему переноса контракта с KZ на CY</li></ul>5) Service Cloud -  Обсуждения возможных способов закупки с вендором (сервис заложен на Q1 2024)6) Highlighting EMIR/SFTR agreeements status & providing test records | 
| top 3-5 points | 
| 0)  **!!!**  Проблема с ресурсами на Проект К. Есть запрос на ресурсы команды Кондор со стороны проекта К. Выделить не можем - нет ресурсов.1) !!! есть проблема с ОХД.Сегодня проводил звонок с ОХД. Пока все очень плохо по ОХД команде 1) менеджмента сейчас по факту нет и\или они не принимают никакого участив в работе с нами. На регулярные встречи они не ходят. Сейчас звонки проходят 1-1 с Катей Кудаевой (аналитик). То есть вся тема по совместной работе стала вырожденной.2) Позиция менеджмента ОХД не понятно, но я предполагаю, что они не считают своей ответственностью управлять бэклогом и связями с командами. Типа если есть проблема, то надо идти к ним, а у них проблем нет. 3) Проблема с разработкой в ОХД. Сейчас есть 3 разработчика в целом на ОХД. Один уходит. Остаются 2 разработчика. Проблема существенная **Заключение**  - мне кажется, что самая тяжелаю проблема по Кипру будет с командой ОХД и их ресурсами.2) Была встреча по статусу эмир-рефита. Коротко можно сказать так:Emir Refit new reportingReady for: FX FWD setup FX SWAP setup CDS on single name setupNOT ready for: EQ OPT setupOut of scope for: OTC EQ/FI FWD setupToDo (somewhere in next phases): CFD3) На этой неделе еще раз актуальной стала проблема с ресурсами команды Кипра (Аналитик и Разработка). Мы почти блокированы и не можем3.1) анализировать проблемы связи НТОЕ-Корт (нет аналитика)3.2) участвовать и обсуждать план действий с командой Кондор по их проекту3.3) планировать доработки для проекта Кондор (переработка сверок, исключение полей, прочее)Как следствие - очень сильно перегружен текучкой Леша В. Это приводит к плохим результатам по ряду направлений. | 
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
| Calypso:<ul><li>BCSCY - продолжаем процесс UAT по Trade / Netting Confirmation. Тестировали смену роли с Custody на CASS client со всеми downstream системами. Делаем аналитику по Liquidity Management Report. Начали тестирование MiFID Transaction репорт в рамках проекта по миграции Кипра. Досетапили продукт CDS для Кипра.</li></ul><ul><li>BCSGL - дали свои оценки по сетапу продукта FX Spot. Сделали багфиксинг и хотфикс по TSL.</li><li>BCSUK - поправили статику для корректного рассчета Accruel Interest по сделкам. По FX разобрали как считается поле TradePrice.</li><li>CASS - исправили в UK ошибки в Position Keeper и Inventory Report по запросам деска UK.</li><li>Тестируем локально развернутый новый инстанс Calypso 17 на NV ресурсом QA. Делаем задачу по исправлению кода, то что нашел Алексей Сидоркин в ходе предварительного анализа.</li></ul>IBQ:<ul><li>Продолжаем делать аналитику по проекту EMIR Refit. Делаем разработку по обработке событий + аналитику по Margin Report.</li><li>Вместе с командой RiskRoom пытаемся определиться с параметрами, которые должны рассчитываться для MarginReport EMIR Refit.</li><li>Новый аналитик на аутсорс, начал заниматься задачей по загрузке данных из Anna DSB в EDW для EMIR Refit проекта.</li><li>Занимались восстановлением тестовой среды QORT, чтобы запустить процесс UAT по задачам релиза.</li></ul>Кондор
1.  **Ресурсная проблема создает огромные риски для проекта перехода на Атриум в этом году.** 
1. Для ИТ руководства обозначены критичные риски проекта перехода на Атриум
1. Проведена встреча с А. Курочкиным (руководитель Систематики) на уровне нашего ИТ руководства. Обозначена наша цель запуститься с || run gateway в мае.
1. !!! Выявлен gap ресурса ИТ ИБ команды БО (Корт) на поддержку проекта перехода на Атриум.

Riskroom:<ul><li>ArmRm - more calrification came to continue ArmRm project</li><li>Email service to implement EWS at EP is ready to go live</li></ul>FX:<ul><li>Dev continues for banded tariffication, delployed to UAT, procedural API for bank agreed, testing stopped at bank side</li><li>New WeekendRates service deployed to UAT</li><li>EWS task: services are being analyzed whether they have email functionality</li></ul>OneTick: Ready to deploy latest changes to EPEMIR/REFIT:<ul><li>More reqs needed</li><li>RR related task (CMA room) - pre-analysis started</li></ul>RegReporting<ul><li>Sorted out major mess at UK, also at UAT</li><li>Continue fixing SC reconciliation service at UK</li><li>None RegT reconciliation service is working properly, and no user demand so far, to investigate further</li><li>Preparing architecture diagram</li></ul>CRM1) Migration of UK CRM service<ul><li>Migration of metadata complete</li><li>Start of data migration</li><li>Preparation for files migration</li><li>Full backup of old data (in case there is no prolongation) </li><li>Switch off letter for old Salesforce org signed and process is started.</li></ul>2) Full CY clientbase upload & support in CRM - providing colleagues with the list of required data with format and comments 3) Обновление справочника ЦФО 2024 - маппинг текущих значений на новые4) Процессинг счета на FormAssembly KZ<ul><li>попытки протолкнуть и найти финансирование в  бюджете</li><li>огранизация встречи с вендором на тему переноса контракта с KZ на CY</li></ul>5) Service Cloud -  Обсуждения возможных способов закупки с вендором (сервис заложен на Q1 2024)6) Highlighting EMIR/SFTR agreeements status & providing test records | 
| top 3-5 points | 
| 0)  **!!!**  Проблема с ресурсами на Проект К. Есть запрос на ресурсы команды Кондор со стороны проекта К. Выделить не можем - нет ресурсов.1) !!! есть проблема с ОХД.Сегодня проводил звонок с ОХД. Пока все очень плохо по ОХД команде 1) менеджмента сейчас по факту нет и\или они не принимают никакого участив в работе с нами. На регулярные встречи они не ходят. Сейчас звонки проходят 1-1 с Катей Кудаевой (аналитик). То есть вся тема по совместной работе стала вырожденной.2) Позиция менеджмента ОХД не понятно, но я предполагаю, что они не считают своей ответственностью управлять бэклогом и связями с командами. Типа если есть проблема, то надо идти к ним, а у них проблем нет. 3) Проблема с разработкой в ОХД. Сейчас есть 3 разработчика в целом на ОХД. Один уходит. Остаются 2 разработчика. Проблема существенная **Заключение**  - мне кажется, что самая тяжелаю проблема по Кипру будет с командой ОХД и их ресурсами.2) Была встреча по статусу эмир-рефита. Коротко можно сказать так:Emir Refit new reportingReady for: FX FWD setup FX SWAP setup CDS on single name setupNOT ready for: EQ OPT setupOut of scope for: OTC EQ/FI FWD setupToDo (somewhere in next phases): CFD3) На этой неделе еще раз актуальной стала проблема с ресурсами команды Кипра (Аналитик и Разработка). Мы почти блокированы и не можем3.1) анализировать проблемы связи НТОЕ-Корт (нет аналитика)3.2) участвовать и обсуждать план действий с командой Кондор по их проекту3.3) планировать доработки для проекта Кондор (переработка сверок, исключение полей, прочее)Как следствие - очень сильно перегружен текучкой Леша В. Это приводит к плохим результатам по ряду направлений. | 







*****

[[category.storage-team]] 
[[category.confluence]] 
