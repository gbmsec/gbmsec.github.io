





| CHG

 | 
| Alexey Dorogov

 | 
| 

 | 
| Calypso:

<ul><li>Продолжаем занимаемся задачей по переходу с FIX сообщений на загрузку из QUIK экспортера. Есть вопросы, которые бы хотелось совместно с командой FO решить.</li><li>Calypso Non UK - готовимся к началу тестирования интеграций в тестовой среде PREPCY. Также определились с наименованиями сред.</li><li>Декомиссия Kondor+ в периметре UK - баг фиксинг по тем замечаниям, которые приходят с прода после разделения потоков.</li></ul>BQ:

<ul><li>Делаем аналитику по проекту EMIR Refit.</li><li>Планируем совместно с Кондор вывести релиз с задачей по переходу с MS MQ на Rabbit MQ в интеграции Кондор - КОРТ. Релиз  </li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>ESB Segregation: RabbitMQ</li><li>QuikExport - Calypso integrations</li></ul>Riskroom:<ul><li>RuData connectivity verified, started working on a service</li><li>Clients/Groups functionality is deployed to prod UK</li><li>Data extractions for FI report was done for Risk analysts</li></ul>FX:<ul><li>Weekend delayed trades: fix delivered</li><li>FINAM report: UAT is ongoing, fixed some issues</li><li>Emergency dashboard bug fix is at UAT</li><li>Started working on adding 2 fields onto Emergency dashboard warning</li></ul>OneTick:<ul><li>delivered functionality for UK to unload files into separate folders by year for OneTick historical data request</li></ul>Кондор
1.  Parallel run этап отключения К+ на UK - неделя, полет нормальный. К нам запросов не поступало. Со стороны Калипсо в очереди ничего не идет.
1. В этом релизе выводим задачу по переводу интеграции с IBQ с MS MQ на ESB.
1. Отключен весь функционал, который был связан с фондированием. Остались таблицы - планируем их удаление.
1. Переход на Атриум - систематизировали наши реестры Codifiers и LightWizards. Договор с Систематикой - возникли расхождения по выплатам 2023 года. В процессе обсуждения. На словах Курочкин согласился (в чате в ватсапе), но письмом пока не подтвердил. 
1. Был проведен kick-off проекта декомиссии Корта. С точки зрения К+ представленный high-level календарный план по К+ не корректен.

Salesforce Non-UK:<ul><li>Testing of integrational push topics</li><li>Setting up Pre-prod Sandbox for SF CY</li><li>Testing Business Processes</li><li>Tesing FormAssembly</li><li>Apex class testing</li><li>Conga Composer - payment/signing process initiated</li></ul> | 
| top 3-5 points | 
| 1) HR подбор - все плохо2) infra:key in (INFRA-4077, INFRA-3323, INFRA-3775, INFRA-4086, INFRA-2661, INFRA-2060, INFRA-4232, INFRA-4103, INFRA-4243, INFRA-4244, INFRA-4224, INFRA-3654, INFRA-4223, INFRA-4153, INFRA-4151, INFRA-4232, INFRA-4151, INFRA-4267, INFRA-4289, INFRA-4293, INFRA-4318)3) Дружинин уходит. Результат - направление Web (NTO, Click) остается без бэкапа совсем4)  **!!!**  Надо ускорить и оперативно оплатить Conga Composer. Заявка заведена5)  **!!!**  Курочкин уже 3 дня не отвечает на вопросы по договру. Согласование заблокировано | 
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
| Calypso:

<ul><li>Продолжаем занимаемся задачей по переходу с FIX сообщений на загрузку из QUIK экспортера. Есть вопросы, которые бы хотелось совместно с командой FO решить.</li><li>Calypso Non UK - готовимся к началу тестирования интеграций в тестовой среде PREPCY. Также определились с наименованиями сред.</li><li>Декомиссия Kondor+ в периметре UK - баг фиксинг по тем замечаниям, которые приходят с прода после разделения потоков.</li></ul>BQ:

<ul><li>Делаем аналитику по проекту EMIR Refit.</li><li>Планируем совместно с Кондор вывести релиз с задачей по переходу с MS MQ на Rabbit MQ в интеграции Кондор - КОРТ. Релиз  </li></ul>ESB<ul><li>ESB internal tasks and bugs</li><li>ESB Segregation: RabbitMQ</li><li>QuikExport - Calypso integrations</li></ul>Riskroom:<ul><li>RuData connectivity verified, started working on a service</li><li>Clients/Groups functionality is deployed to prod UK</li><li>Data extractions for FI report was done for Risk analysts</li></ul>FX:<ul><li>Weekend delayed trades: fix delivered</li><li>FINAM report: UAT is ongoing, fixed some issues</li><li>Emergency dashboard bug fix is at UAT</li><li>Started working on adding 2 fields onto Emergency dashboard warning</li></ul>OneTick:<ul><li>delivered functionality for UK to unload files into separate folders by year for OneTick historical data request</li></ul>Кондор
1.  Parallel run этап отключения К+ на UK - неделя, полет нормальный. К нам запросов не поступало. Со стороны Калипсо в очереди ничего не идет.
1. В этом релизе выводим задачу по переводу интеграции с IBQ с MS MQ на ESB.
1. Отключен весь функционал, который был связан с фондированием. Остались таблицы - планируем их удаление.
1. Переход на Атриум - систематизировали наши реестры Codifiers и LightWizards. Договор с Систематикой - возникли расхождения по выплатам 2023 года. В процессе обсуждения. На словах Курочкин согласился (в чате в ватсапе), но письмом пока не подтвердил. 
1. Был проведен kick-off проекта декомиссии Корта. С точки зрения К+ представленный high-level календарный план по К+ не корректен.

Salesforce Non-UK:<ul><li>Testing of integrational push topics</li><li>Setting up Pre-prod Sandbox for SF CY</li><li>Testing Business Processes</li><li>Tesing FormAssembly</li><li>Apex class testing</li><li>Conga Composer - payment/signing process initiated</li></ul> | 
| top 3-5 points | 
| 1) HR подбор - все плохо2) infra:key in (INFRA-4077, INFRA-3323, INFRA-3775, INFRA-4086, INFRA-2661, INFRA-2060, INFRA-4232, INFRA-4103, INFRA-4243, INFRA-4244, INFRA-4224, INFRA-3654, INFRA-4223, INFRA-4153, INFRA-4151, INFRA-4232, INFRA-4151, INFRA-4267, INFRA-4289, INFRA-4293, INFRA-4318)3) Дружинин уходит. Результат - направление Web (NTO, Click) остается без бэкапа совсем4)  **!!!**  Надо ускорить и оперативно оплатить Conga Composer. Заявка заведена5)  **!!!**  Курочкин уже 3 дня не отвечает на вопросы по договру. Согласование заблокировано | 







*****

[[category.storage-team]] 
[[category.confluence]] 
