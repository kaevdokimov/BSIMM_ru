# BSIMM_ru
Краткий перевод BSIMM (https://www.bsimm.com) на русский язык

### Термины

Группа обеспечения безопасности программного обеспечения (SSG):  внутренняя группа, отвечающая за обеспечение и обеспечение безопасности программного обеспечения. Первым шагом инициативы безопасности программного обеспечения (SSI) является формирование SSG.

Инициатива по обеспечению безопасности программного обеспечения (SSI):  общеорганизационная программа для скоординированного внедрения, измерения, управления и развития мероприятий по обеспечению безопасности программного обеспечения.

Спутник (satellite):  группа заинтересованных сотрудников, например разработчиков, архитекторов, менеджеров программного обеспечения, тестировщиков и людей с похожими ролями, которые имеют интерес к безопасности программного обеспечения и задействованы группой безопасности программного обеспечения (SSG).

## Управление - стратегия и метрики 
https://www.bsimm.com/framework/governance/software-security-metrics-strategy.html


#### Уровень 1

##### [SM1.1: 81] Опубликовать процесс и развиваться по мере необходимости.

Процесс решения проблем безопасности программного обеспечения публикуется и передается всем заинтересованным сторонам, так чтобы все знали общий план. Цели, роли, обязанности и действия должны быть четко определены в команде.

##### [SM1.2: 66] Создать роль евангелиста и проводить внутренний маркетинг.

Евангелист может помочь команде внедрить более эффективные методы обеспечения безопасности программного обеспечения при переходе к гибкой методологии. Евангелисты нужны для улучшения понимания и завоевания доверия, проводя беседы с внутренними группами (включая руководителей), рассылая приглашения известным экспертам, готовя официальные документы для внутреннего потребления или создавая набор документов, книг и других ресурсов на внутреннем веб-сайте.

##### [SM1.3: 73] Обучать руководителей.

Руководителям периодически необходимо демонстрировать последствия и влияние неадекватной безопасности программного обеспечения для бизнеса. Привязка обучения к конкретным областям разработки, таким как мобильные или облачные сервисы, или к конкретным методологиям, таким как CI / CD и DevOps, также может помочь убедить руководство принять рекомендации SSG, когда их можно было бы игнорировать в пользу более быстрых дат выпуска или других приоритетов.

##### [SM1.4: 107] Определить гейты, собрать необходимые артефакты.
Идентифицировать заранее гейты безопасности.  Первые два шага на пути к созданию гейтов, специфичных для безопасности - определить местоположения гейтов, которые совместимы с существующими практиками разработки, а затем начать собирать данные, необходимые для принятия решения о том, что может использоваться для прохождения гейтов, а что нет. 

#### Уровень 2
##### [SM2.1: 49] Внутренняя публикация данных о безопасности программного обеспечения.

Чтобы облегчить улучшение, SSG публикует внутренние данные о состоянии безопасности программного обеспечения в организации. Эта информация может быть представлена ​​в виде информационной панели с метриками для руководителей и управления разработкой программного обеспечения. Иногда эти опубликованные данные не будут передаваться всем сотрудникам компании, а только соответствующим руководителям, которые затем приведут к изменениям в организации. 

##### [SM2.2: 53] Применить к контролю гейтов измерение и отслеживание исключений.

Определение условия прохождения гейтов безопасности. Для прохождения гейта проект должен либо соответствовать установленным мерам, либо получить отказ. Разрешение на автоматическое прохождение любых проектов или автоматическое предоставление исключений без должного рассмотрения отрицательно сказывается на применении принудительных мер. В некоторых случаях гейты напрямую связаны с правилами, договорными соглашениями и другими обязательствами, за исключением случаев, которые отслеживаются в соответствии с требованиями законодательных или регулирующих драйверов.

##### [SM2.3: 52] Создать или вырастить спутников (satellite).

Создайте группу людей, разбросанных по всей организации, которые демонстрируют интерес к безопасности приложений, либо имеют навыки  выше среднего - спутникам. Формирование этой группы, иногда называемых чемпионами, является шагом к созданию сети людей, которая ускоряет внедрение безопасности в разработку программного обеспечения. Одним из способов создания начальной группы является отслеживание людей, которые выделяются во время вводных учебных курсов; см. [ T3.6. Определить новых спутниковых участников посредством обучения]. Другой способ - попросить добровольцев.

##### [SM2.6: 51] Требовать подтверждения для принятия рисков безопасности.

В организации имеется тот, кто подтверждает наличие риска и  подписывает состояние всего ПО до его релиза. Политика подтверждения (подписания) рисков может потребовать от руководителя подразделения, например, подписаться на критические уязвимости, которые не были устранены, или на шаги SSDL, которые были пропущены. Политика подписания должна применяться как к внешним проектам, таким как мобильное приложение, так и к проектам, которые будут развернуты во внешних средах, таких как облако. Само по себе принятие риска без формального подтверждения не является подтверждением безопасности, поскольку акт принятия риска более эффективен, когда он формализован (например, с подписью, отправкой формы или чем-то подобным) и собран для последующего использования. Так же, простое заявление о том, что некоторые проекты вообще не требуют одобрения, не приведет к желаемым результатам управления рисками.

#### Уровень 3

##### [SM3.1: 21] Используйте внутреннюю систему для отслеживания

SSG использует автоматизированную систему для централизованного отслеживания прогресса каждого компонента программного обеспечения, независимо от методологии разработки. Автоматизация регистрирует запланированные, выполняемые и завершенные действия по обеспечению безопасности, включая результаты таких действий, как анализ архитектуры, анализ кода и тестирование безопасности, даже если они происходят в тесном цикле. Комбинированный подход к инвентаризации и оценке рисков является основополагающим. SSG использует автоматизацию для создания отчетов по нескольким показателям и во многих случаях публикует эти данные, по крайней мере, среди руководителей.

##### [SM3.2: 6] Запустить внешнюю маркетинговую программу.

SSG может публиковать статьи или книги о возможностях обеспечения безопасности своего программного обеспечения или вести публичный блог. Также SSG может предоставить информацию на внешних конференциях или выставках. В некоторых случаях полная методология SSDLС может быть опубликована и продвигаться за пределами компании, при этом в проектах по безопасности для мобильных устройств, облачных технологий и новых технологий проводятся важные тематические исследования по безопасности программного обеспечения. 

##### [SM3.3: 14] Определить показатели и использовать их для управления бюджетом.

SSG и его руководство выбирают метрики, которые определяют и измеряют прогресс в количественном выражении. Эти показатели, в свою очередь, определяют бюджет инициативы и распределение ресурсов, поэтому простых подсчетов и измерений вне контекста здесь будет недостаточно. Одним из таких показателей может быть плотность дефектов безопасности, сокращение которой можно использовать для уменьшения затрат на восстановление с течением времени. Напомним, что в гибких методологиях метрики лучше собирать на ранних этапах и часто облегченным способом. Ключ заключается в том, чтобы связать технические результаты с бизнес-целями ясным и очевидным способом, чтобы оправдать финансирование. 

##### [SM3.4: 0] Интегрировать программное управление жизненным циклом.

Организации начинают заменять традиционное управление жизненным циклом документов, презентаций и электронных таблиц программными платформами доставки. Люди, которым помогают инструменты, больше не ведут прогресс с каждой фазы жизненного цикла на следующую. Вместо этого организации полагаются на автоматизацию для управления процессом управления и доставки с помощью программного обеспечения ALM / ADLM, такого как Spinnaker

## Управление - соответствие требованиям и ведение политик
https://www.bsimm.com/framework/governance/compliance-and-policy.html

#### Уровень 1

##### [CP1.1: 81] Унифицировать нормативное давление.

Если бизнес или его клиенты подчиняются нормативным драйверам, таким как стандарты безопасности индустрии платежных карт; GLBA, SOX и HIPAA в Соединенных Штатах; или GDPR в ЕС, то SSG выступает в качестве координационного центра для понимания ограничений, которые такие драйверы накладывают на программное обеспечение. В некоторых случаях SSG создает или сотрудничает на основе унифицированного подхода, который устраняет избыточность и конфликты из перекрывающихся требований соответствия. Унифицированный набор руководств по безопасности программного обеспечения для соответствия нормативным требованиям обеспечивает максимально эффективное выполнение работы по обеспечению соответствия.

##### [CP1.2: 105] Определить требования для обработки ПДн.

SSG играет ключевую роль в определении и описании обязательств при обработки ПДн, вытекающих из нормативных требований и ожиданий клиентов, путем использования этой информации для продвижения лучших практик, связанных с конфиденциальностью. То, как программное обеспечение обрабатывает ПДн, должно быть четко регламентировано, но даже если это не так, то конфиденциальность должна являться горячей темой. 

##### [CP1.3: 76] Написать политику безопасности

SSG направляет организацию, создавая или внося вклад в политику безопасности программного обеспечения, которая удовлетворяет внутренним, нормативным требованиям и требованиям безопасности. Эта политика включает унифицированный подход для удовлетворения списка драйверов безопасности на уровне управления. В результате, проектным группам становится необзятельно знать всех деталей, связанных с соблюдением всех применимых правил (нормативные акты, требования безопасности клиента). Им достаточно придерживаться существующей политике. Политика может охватывать требования к обработке ПДн, требования криптографии, либо быть связана с SDLC и его использованию в организации. Точно так же может потребоваться, например, объяснить, что можно и нельзя автоматизировать в CI / CD и в конвейерах непрерывного развертывания (см. [SM3.4 Интеграция программно-определяемого управления жизненным циклом]). При этом стандарты архитектуры и руководства по разработке не являются примерами политики. Политика - это то, что разрешено и запрещено; если это не обязательно, это не политика. Во многих случаях заявления о политике должны быть переведены в автоматизацию для использования в жизненном цикле, а не просто как процесс, навязываемый людьми, но даже автоматизированная политика должна быть обязательной.

#### Уровень 2

##### [CP2.1: 48] Определить перечень ПДн .

Организация определяет виды ПДн, обрабатываемые или хранимые каждой из своих систем, а также связанные с ними хранилища данных. Инвентаризировать ПДн можно двумя способами: начиная с каждого отдельного приложения, отмечая обрабатываемое им ПДн или начиная с определенных видов ПДн и отмечая приложения, которые их касаются. Поддержание инвентаризации затрудняется за счет перетекания приложения в облачные среды.

##### [CP2.2: 47] Требовать подтверждения безопасности для риска, связанного с соблюдением соответствия.

В организации существует формальный процесс принятия рисков, который охватывает все проекты разработки программного обеспечения. В этом процессе SSG выступает в роли советника, когда ответственный за принятие риска подписывает состояние программного обеспечения до его выпуска.  Например, политика подписи может потребовать от руководителя подразделения подписать вопросы, которые не были устранены, или пропущенные шаги SSDL, связанные с соблюдением соответствия. Подписание должно быть явным и регистрироваться для использования в будущем, с любыми отслеживаемыми исключениями, даже при использовании самой быстрой из гибких методологий. В тех случаях, когда ответственный за принятие риска подписывает определенный набор критериев приемлемости соответствия, которые затем внедряются с помощью средств автоматизации, должна проводиться постоянная проверка того, что критерии остаются точными, и автоматизация фактически работает.

##### [CP2.3: 51] Внедрить и отслеживать меры контроля на соответствие.

Организация может продемонстрировать соответствие применимым требованиям, поскольку ее SDLC соответствует утвреждениям, разработанным SSG (см. [ CP1.1 Унифицировать нормативное давление ]). SSG контролирует проблемные области SDLC и обеспечивает удовлетворение аудиторов и регулирующих органов. Подход DevOps к внедрению средств управления соответствием в процесс все чаще проявляется в программно-определяемой инфраструктуре, а не в ручном вмешательстве.  

##### [CP2.4: 44] Включить SLA безопасности программного обеспечения во все контракты с поставщиками.

Контракты с поставщиками должны включать SLA, чтобы гарантировать, что поставщик не мог поставить под угрозу обеспечение соотвтествия организации (историю соответствия). Каждый новый или возобновленный контракт должен содержать положения, требующие от поставщика решения вопросов безопасности программного обеспечения и предоставления продукта или услуги, совместимых с политикой безопасности организации (см. [ SR2.5 Создание шаблона SLA ]). Традиционные требования к ИТ-безопасности и простое соглашение, разрешающее тестирование на проникновение, здесь недостаточны.

##### [CP2.5: 56] Обеспечить осведомленность руководителей об обязательствах по соблюдению и конфиденциальности.

Чтобы привлечь внимание руководства к соблюдению нормативных требований и конфиденциальности, SSG предоставляет руководителям понятные объяснения обязательств организации по соблюдению конфиденциальности, а также возможные последствия невыполнения этих обязательств. Для некоторых организаций объяснение прямых затрат и вероятных последствий несоблюдения или утечки данных является эффективным способом обсуждения этой темы. Для других будет эффективным привлечение внешнего эксперта.

#### Уровень 3

##### [CP3.1: 25] Создать историю соответствия регуляторам.

У SSG есть информация, которую хотят регуляторы, поэтому комбинация письменной политики, управляющей документации и артефактов, собранных с помощью SSDL, дает SSG возможность продемонстрировать историю соответствия организации без подробного анализа для каждого аудита. Часто регуляторы, аудиторы и высшее руководство будут удовлетворены теми же видами отчетов, которые могут быть получены непосредственно из различных инструментов. В некоторых случаях организации потребуется дополнительная информация от поставщиков о том, как средства управления поставщика поддерживают потребности организации в соответствии (например, облачные провайдеры, особенно в мульти-облачном развертывании). 

##### [CP3.2: 15] Установить политику для поставщиков.

Поставщики обязаны придерживаться тех же политик, которые используются внутри компании, и должны представить доказательства того, что их практика обеспечения безопасности программного обеспечения прошла проверку. Это могут быть поставщики облачных услуг, поставщики промежуточного программного обеспечения, поставщики виртуализации, контейнеров и оркестрации, создатели программного обеспечения, подрядчики и многие другие, и каждый из них может придерживаться различных требований политики. Доказательства их соответствия могут включать результаты проверок кода или тестов на проникновение или тестов, встроенных непосредственно в автоматизацию или инфраструктуру. В некоторых случаях оценка BSIMM или оценка BSIMMsc может помочь гарантировать, что поставщики соблюдают политики безопасности программного обеспечения фирмы.

##### [CP3.3: 7] Подвергать политику изменениям благодаря обратной  связи

Политика должна поддаваться изменениям. Регулярное появление неадекватного анализа архитектуры, повторяющихся уязвимостей, игнорируемых гейтов безопасности или неправильного выбора компании для проведения теста на проникновение может выявить слабость политики. В некоторых случаях данные жизненного цикла могут указывать на то, что политики навязывают слишком много бюрократии, например, появляются разногласия, которые мешают соответствовать ожидаемой частоте доставки. Быстрое развитие технологий может также создать пробелы в политике, которые необходимо устранить. Со временем политика становится более практичной и ее легче проводить (см. [SM1.1 Опубликуйте процесс и развивайтесь по мере необходимости ]). В конечном итоге политики уточняются данными SSDL для повышения эффективности организации. 
