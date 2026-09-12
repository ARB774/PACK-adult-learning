# Pack Manifest: Adult Learning and Continuing Professional Education
## Metadata
```yaml
pack_id: AL
pack_name: Проектирование обучения взрослых и программ ДПО
pack_name_en: Adult Learning and Continuing Professional Education Design
version: 0.1.0
fpf_edition: 56440a9f2e252d7fd462f43470a433dd03413e19
fpf_edition_date: 2026-09-05
architecture_decision: DPF-DRR.md
pilot_edition_ref: DPF-EDITION@pilot-2026-09-04.24
pilot_edition_record: DPF-EDITION.md
relation_maintenance_record: DPF-PFR.md
pilot_selected_patterns: [AL.P.001, AL.P.002, AL.P.003, AL.P.004, AL.P.005, AL.P.006, AL.P.007, AL.P.008, AL.P.009, AL.P.010, AL.P.011, AL.P.012, AL.P.013, AL.P.014, AL.P.015, AL.P.016, AL.P.017, AL.P.018, AL.P.019, AL.P.020, AL.P.021, AL.P.022, AL.P.023, AL.P.024]
public_name: not_selected
publication_occurrence: not_asserted
pilot_evaluation_status: admissibleForDeclaredDPFUse
pilot_evaluation_floor: 3
spf_template_checked: 2026-07-28
status: draft
created: 2026-07-28
last_updated: 2026-09-12
maintainers:
  - name: Workspace owner
    contact: local
```
## Scope
Pack отвечает на вопросы:
- какие особенности взрослого обучающегося значимы для проектирования;
- как связать образовательный запрос, опыт, практику, рефлексию и перенос в работу;
- какие роли, методы и проверяемые рабочие продукты образуют практику проектирования обучения взрослых;
- как проектировать программы ДПО с индивидуализацией, сопровождением и партнёрством с рынком труда;
- какие типовые отказы снижают результативность и как их обнаруживать.
Не входят:
- готовая программа конкретного курса, календарный план и расписание;
- нормативно-правовая экспертиза лицензирования и реализации ДПО;
- выбор конкретной LMS, поставщика ИИ, VR/AR-оборудования или платформы;
- клиническая психология, психотерапия и медицинская реабилитация;
- обучение детей и подростков;
- кадровая стратегия конкретной организации.
- структурирование неустановленной системной проблемы и подготовка рекомендации владельцу выбора — это соседний домен PSD;
- проектирование границы, позиций, полномочий и отношений изменённой организации — это соседний домен OCE.
- общий индивидуальный контур развития способности для будущей работы — от
  требования и диагностики до выбора программы, проверки переноса, сохранения и
  пересмотра — принадлежит HCD; Pack поставляет специализированные методы
  обучения взрослых и отдельно удерживает коллективное научение в
  трансформации.
## Object of description
Объект описания — воспроизводимые специализированные методы обучения взрослых:
работа с опытом, авторством, рефлексией, ошибкой, помощью, учебной пробой,
развивающим переходом и коллективным научением. Общий индивидуальный контур
развития способности для будущей работы и итоговые выводы о способности,
переносе, сохранении и зависимости от поддержки принадлежат HCD.
## Dependencies
| FPF/SPF distinction | Use in this Pack |
|---|---|
| Method ≠ tool | Метод описывает воспроизводимый способ получения результата; инструмент лишь поддерживает его |
| Work product ≠ activity | Рабочий продукт — наблюдаемый и проверяемый выход деятельности |
| Role ≠ person/job title | Один человек может занимать несколько функциональных ролей |
| Characteristic ≠ indicator | Характеристика — что оценивается; индикатор — наблюдаемый признак |
| Pack ≠ downstream solution | Pack описывает домен; конкретный курс и его реализация находятся ниже по стеку |

### Межпакетная зависимость

| Pack | Отношение |
|---|---|
| Pack-ATB | При признанном хроническом разрыве результативности выступает владельцем заказа на способность: определяет исполнителей, требуемые действия, пересматриваемые основания, изменения контекста и системный результат. Pack-adult-learning принимает этот заказ, проверяет образовательный разрыв, проектирует научение и возвращает раздельные свидетельства способности; неполное или противоречивое требование возвращается в Pack-ATB. |
| Pack-TOC | `AL.P.001`, `AL.P.008`, `AL.P.012`, `AL.P.015` и прежде всего `AL.P.017` не выявляют ограничивающее убеждение собственным методом. Они передают наблюдаемое расхождение и обе стороны конфликта в Pack-TOC: `TOC.M.003` строит полную тучу, `TOC.M.004` опознаёт кандидата в ограничивающее предположение, `TOC.M.009` проверяет конфликт заявленной и фактической линии действия, а `TOC.D.006` отделяет предположение от элемента тучи. Точная опора: коммит `44c876e1f58b50e61b2625a927890a3791b99532`. |
| PSD DPF | Получает запрос, когда до образовательной диагностики нужно удержать несколько формулировок проблемы, участников, ценности, альтернативы и неопределённость и подготовить рекомендацию владельцу выбора. Рекомендация не создаёт решение или мандат. |
| OCE DPF | Получает обоснованную неучебную часть, когда рабочая проба требует изменить роли, полномочия, отношения вкладов или устройство продолжающейся работы. План переноса не заменяет инженерное получение организации. |
| HCD DPF | Владеет общим индивидуальным контуром развития способности для представительной будущей работы. Передаёт Pack названного взрослого, требуемый вклад, квалифицированный объект развития, текущую конфигурацию выполнения, условия участия и вопрос выбора специализированного метода. Получает от Pack взрослый образовательный механизм, требования к опыту, авторству, помощи, обратной связи, пробе и безопасности, наблюдения учебного эпизода и ограничения вывода. HCD отдельно принимает решение о программе и квалифицирует способность, перенос, сохранение и зависимость от инструментов. |
| RMP DPF | Владеет исследовательским результатом: квалифицирует нерешённый вопрос (`RMP.1`), выбирает критикуемый дизайн (`RMP.2`), превращает его в исполнимый протокол (`RMP.3`) и сохраняет проверяемый след фактического исследования (`RMP.4`). Pack владеет обучением взрослых и групп, включая учебные циклы исследования действием. Сбор данных, рефлексия и рабочие пробы не становятся исследованием без отдельного RMP-результата; RMP не устанавливает освоение, перенос или организационное изменение. |
## Content summary
| Section | Count | Status |
|---|---:|---|
| Distinctions | 14 | draft |
| Roles | 7 | draft |
| Objects of attention | 10 | draft |
| Methods | 10 | draft |
| Work products | 10 | draft |
| Failure modes | 10 | draft |
| Characteristics | 8 | draft |
| SoTA annotations/source groups | 29 | draft |
| Maps | 1 | draft |
## Entity index
| ID | Name | Kind | Summary | Status |
|---|---|---|---|---|
| AL.M.001 | Диагностика образовательного запроса | M | Связывает цели взрослого, контекст труда, опыт, ограничения и требуемый результат | draft |
| AL.M.002 | Проектирование цикла «опыт — осмысление — действие | M | Превращает опыт и практическое действие в переносимое знание | draft |
| AL.M.003 | Проблемно-кейсовое обучение | M | Организует освоение через реалистичную проблему или кейс | draft |
| AL.M.004 | Поддержка самонаправленного обучения | M | Настраивает объём выбора и опоры по готовности обучающегося | draft |
| AL.M.005 | Тьюторское сопровождение траектории | M | Помогает удерживать запрос, рефлексию и следующий карьерно-образовательный шаг | draft |
| AL.M.006 | Проектирование переноса в рабочую практику | M | Встраивает применение, поддержку и проверку результата после обучения | draft |
| AL.M.007 | Оценивание эффектов обучения | M | Собирает доказательства обучения, поведения и контекстных результатов | draft |
| AL.M.008 | Экосистемное проектирование ДПО | M | Связывает необходимые вклады сторон, проверяемые переходы, полномочия, данные и устойчивость конфигурации | draft |
| AL.M.009 | Проектирование развивающего перехода | M | Связывает пересмотр основания с авторизованной пробой, изменением «Я — Мы — Это» и проверкой жизнеспособности | draft |
| AL.M.010 | Маршрутизация образовательного запроса | M | Проверяет происхождение целевого действия, выбирает исходный домен и допускает переход к образовательной диагностике | draft |
| AL.WP.001 | Профиль образовательного запроса | WP | Проверяемое описание цели, опыта, контекста и ограничений | draft |
| AL.WP.002 | Карта результатов и компетенций | WP | Связывает действия, критерии и доказательства освоения | draft |
| AL.WP.003 | Архитектура учебного опыта | WP | Отображает последовательность опыта, рефлексии, концептуализации и действия | draft |
| AL.WP.004 | Практическое задание | WP | Задание, имитирующее или выполняющее реальную деятельность | draft |
| AL.WP.005 | Критериальная шкала оценки и план доказательств | WP | Фиксирует критерии качества и допустимые свидетельства | draft |
| AL.WP.006 | План индивидуальной траектории и сопровождения | WP | Описывает выбор, опоры, контрольные точки и пересмотр маршрута | draft |
| AL.WP.007 | План переноса в рабочую практику | WP | Фиксирует применение, среду, поддержку и проверку после обучения | draft |
| AL.WP.008 | Отчёт об эффектах | WP | Сводит данные об участии, освоении, поведении и результатах контекста | draft |
| AL.WP.009 | Карта развивающего перехода | WP | Описывает глубину результата, основание и его функцию, проверяемый диалог, альтернативу и план, способности, авторство, мандат, пробу, поддержку среды, «Я — Мы — Это», жизнеспособность и уровни результата | draft |
| AL.WP.010 | Паспорт основания и маршрута образовательного запроса | WP | Трассирует источник системного основания, мандат, образовательную часть, маршрут, риск и неопределённость | draft |
## Maturity and gaps
Версия 0.1 пригодна для поиска, проектной ориентации и подготовки следующих итераций. Для статуса `active` нужны:
1. экспертная проверка практиками ДПО и корпоративного обучения;
2. отдельный обзор действующих нормативных требований;
3. расширение первичных исследований по эффективности методов;
4. проверка терминов на пересечение с соседними Pack;
5. апробация рабочих продуктов минимум в двух программах;
6. фиксация метрик до/после и revision criteria по каждой SoTA-аннотации.
## Change log

| Date | Change | Author |
|---|---|---|
| 2026-09-12 | Completed post-integration ODI boundary review with 10 new synthetic cases; all resolved using explicit rules; no entity changes required; same-agent analytical review, not independent or empirical validation; candidate/bounded unchanged | Codex |
| 2026-09-12 | Integrated ODI supplementary claims 035–043 into AL.P.027, AL.M.002, AL.M.009 and AL.WP.009 using existing architecture; 43 accepted claims; pattern remains candidate/bounded; post-integration boundary tests pending | Codex |
| 2026-09-12 | Owner accepted plain-language STH.ODI.CLAIM.043 as bounded; all 43 claims accepted; supplementary claims 035–043 await integration | Codex |

| 2026-09-12 | Owner accepted STH.ODI.CLAIM.042 as bounded on mutual determination; source account and Pack rule remain separate; 42 accepted, 1 pending; not yet integrated | Codex |

| 2026-09-12 | Owner accepted STH.ODI.CLAIM.041 as bounded for P. G. Shchedrovitsky's model; 41 accepted, 2 pending; not yet integrated | Codex |

| 2026-09-12 | Owner accepted STH.ODI.CLAIM.040 as bounded; source function and Pack safe adaptation remain separate; 40 accepted, 3 pending; not yet integrated | Codex |

| 2026-09-12 | Owner accepted STH.ODI.CLAIM.039 as bounded for the author's ODI model; 39 accepted, 4 pending; not yet integrated | Codex |

| 2026-09-12 | Owner accepted refined STH.ODI.CLAIM.038 as bounded; distinguished source mechanism from Pack procedure; 38 accepted, 5 pending; not yet integrated | Codex |

| 2026-09-12 | Owner accepted refined STH.ODI.CLAIM.037 as current-practice; distinguished schemed thinking from work coordination and source meaning from Pack concretization; 37 accepted, 6 pending | Codex |
| 2026-09-12 | Owner accepted STH.ODI.CLAIM.036 as current-practice for use and coordination of multiple representations; 36 accepted, 7 pending; integration pending | Codex |
| 2026-09-12 | Owner accepted STH.ODI.CLAIM.035 as bounded; recorded separate TOC-cloud comparison as Pack synthesis; 35 accepted, 8 pending, integration pending | Codex |
| 2026-09-12 | Formulated source-near STH.ODI.CLAIM.035–043 for owner review; 34 accepted and 9 pending claims, 34 works unchanged; no pattern integration | Codex |
| 2026-09-12 | Added STH.ODI.031–034 and source-fragment comparison to reopened AL.SOTA.027; cycle corpus now 34 works, accepted claims unchanged; procedural saturation remains open | Codex |
| 2026-09-12 | Reopened AL.SOTA.027 to check source-near mechanisms of schematization, objectivation, positioning and problematization; preserved accepted claims and pattern status; no new cycle or source count change | Codex |
| 2026-09-12 | Corrected SoTA annotation/source-group count from 28 to 29 to include registered AL.SOTA.029 | Codex |
| 2026-09-12 | Integrated all 34 accepted Schön claims into existing distinctions, methods, five patterns and work products; preserved 29 current-practice, 4 bounded and 1 modern-AI hypothesis; broader coaching source check remains open; no new entity or pilot-edition claim | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.022` as current practice: replace a generic reflection instruction with an explicit object, learner actions, work product, intended change, and next probe | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.023` as bounded: reflective writing supports formative feedback but cannot by itself prove acquired capability or changed practice | Codex |
| 2026-09-12 | Accepted `STH.SCH.CLAIM.034` as current practice: investigate learning binds through reciprocal reflection on interaction, including the coach's assumptions; all 34 claims accepted, primary coaching-mode comparison still open | Codex |
| 2026-09-12 | Accepted `STH.SCH.CLAIM.033` as current practice: collaborative coaching preserves learner authorship, explores alternative means and evaluates intended qualities within the declared task and source-case boundary | Codex |
| 2026-09-12 | Accepted `STH.SCH.CLAIM.032` as current practice: reflection-in-action enriches the professional repertoire; preserve Pack's experience-recording proposal as a separate synthesis | Codex |
| 2026-09-12 | Accepted `STH.SCH.CLAIM.031` as current practice: use prior examples without erasing the new case's uniqueness, test the transferred move in action, and distinguish Pack's teaching questions from Schon's account | Codex |
| 2026-09-12 | Accepted `STH.SCH.CLAIM.030` as current practice: assess the practical move and its full consequences separately from the explanation; preserve the limits of inference from one trial | Codex |
| 2026-09-12 | Accepted `STH.SCH.CLAIM.029` as current practice: distinguish exploratory, move-testing and hypothesis-testing functions while preserving their possible combination in one practical move | Codex |
| 2026-09-12 | Formulated source-near `STH.SCH.CLAIM.029–034` from existing Schon works on experiment functions, outcome logic, repertoire, collaborative coaching and learning binds; 28 accepted, 6 pending, 32 independent works unchanged | Codex |
| 2026-09-12 | Accepted `STH.SCH.CLAIM.028` as a modern AI-use hypothesis, not Schon's teaching; rechecked saturation and identified method-detail gaps in experimentation, repertoire, and coaching; integration remains pending | Codex |
| 2026-09-12 | Accepted `STH.SCH.CLAIM.027` as current practice: preserve Argyris and Schon's joint account of double-loop learning and separate Pack's subsequent-action verification requirement | Codex |
| 2026-09-12 | Accepted `STH.SCH.CLAIM.026` as current practice: reframing opens reconsideration, while action, result verification, and consolidation belong to Pack's synthesis | Codex |
| 2026-09-12 | Accepted `STH.SCH.CLAIM.025` as current practice: preserve Schon and Rein's public-policy scope and distinguish Pack's application to collective learning | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.024` as bounded: reflective work must guard against rumination and return the learner to evidence, influence, and a safe next action | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.021` as current practice: require speaking safety, authority to change joint work, and a subsequent test for team reflection | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.020` as current practice from later research: treat team reflexivity as joint review and revision of goals, coordination, roles, and work methods | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.019` as current practice: use a compact action–debrief–change–reattempt cycle when action data and a comparable next attempt are available | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.018` as bounded: transfer structured hypothesis comparison as a design hypothesis while retaining the direct evidence boundary in medical diagnosis | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.017` as bounded: reserve extended structured reflection for complex, uncertain, surprising, or competing-explanation cases | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.016` as a Pack-inference current practice: treat changed subsequent action as the main reflection evidence and reflective text as intermediate evidence | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.015` as corpus-synthesis current practice: make critique specific to intent, move, product, consequence, and the next attempt | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.014` as current practice with a domain boundary: specify the work material and perceptual distinctions that guide the next professional move | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.013` as current practice: permit initial imitation as temporary support, then fade the model and test independent choice in a new situation | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.012` as current practice: alternate early attempts with demonstration, explanation, and clarifying dialogue | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.011` as current practice: require a practicum coach to make expert distinctions and moves observable and connect critique to the learner's next attempt | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.010` as current practice: make learner moves, evolving work products, consequences, help, and revisions the practicum material | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.009` as current practice with explicit practicum boundaries: state represented and omitted work conditions and require a workplace transfer probe | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.008` as current practice: develop professional artistry through situated action, observation, dialogue, consequences, and repeated attempts | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.007` as current practice: distinguish reflection during action from reflection after action and test the latter in a subsequent attempt | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.006` as current practice: use observable consequences as the situation's response while testing the practitioner's interpretation | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.005` as current practice: make problem framing and system boundary explicit and testable before evaluating the proposed solution | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.004` as current practice: structure reflection-in-action as reframing followed by a probe and observation of consequences | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.003` as current practice: use observable surprise, not a generic request to reflect, to trigger reflection-in-action | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.002` as current practice: elicit tacit professional knowing from observable action and products without treating intuition as automatically correct | Codex |
| 2026-09-11 | Accepted `STH.SCH.CLAIM.001` as current practice: technical knowledge is insufficient where the professional must first frame an indeterminate, unique, or conflicted situation | Codex |
| 2026-09-11 | Formulated `STH.SCH.CLAIM.001–028` from the 32-source Schön corpus without a preset count; separated source claims, joint Argyris–Schön claims, research findings, and Pack inferences | Codex |
| 2026-09-11 | Harvested 32 independent sources across 12 streams for `AL.SOTA.029`; separated Schön's primary model, joint Argyris–Schön works, empirical tests, critiques, collective reflection, and early AI support | Codex |
| 2026-09-11 | Opened `AL.SOTA.029` on Donald Schön's reflective practice; separated Schön's own professional-learning line from joint Argyris–Schön work and registered 12 source streams without drafting claims | Codex |
| 2026-09-11 | Integrated all 26 accepted Knowles claims into existing roles, methods, work products, patterns and DPF; closed four architectural gaps without adding entities and represented the learning contract as a linked view of existing work products | Codex |
| 2026-09-11 | Accepted `STH.KNW.CLAIM.026` as Pack-AL `current-practice`: preserve only the honestly available learner choices in short mandatory corporate programs; all 26 Knowles claims are now reviewed and integration remains pending | Codex |
| 2026-09-11 | Accepted `STH.KNW.CLAIM.025` as Pack-AL `current-practice`: retain Knowles's andragogical conditions but add a separate route for testing, changing and enacting activity grounds; organizational causes route to Pack-ATB | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.024` as `bounded`: Knowles's diagnostic exercises with performance feedback can prepare reconsideration of activity grounds but do not constitute a complete method for changing them | Codex |
| 2026-09-11 | Accepted cross-domain synthesis `STH.KNW.CLAIM.023` as `current-practice`: route individual, collective and organizational causes separately instead of assigning every contextual gap to collective learning | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.022` as `current-practice`: Knowles's later pedagogical-andragogical models are selected for situational fit rather than age alone and will be integrated through existing `CLAIM.003` | Codex |
| 2026-09-11 | Accepted corpus-synthesis `STH.KNW.CLAIM.021` as `current-practice`: an andragogy label does not establish superiority, so evidence use names concrete mechanisms, results and conditions | Codex |
| 2026-09-11 | Accepted `STH.KNW.CLAIM.020` as `bounded` for Knowles's preference for internal motivation and as `current-practice` for Pack-AL's separate requirement to inspect the actual motivational situation | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.019` as `current-practice`: application is planned and rehearsed during learning while actual transfer remains a separate later conclusion | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.018` as `current-practice`: the learner proposes evidence and verification without self-certifying mastery; recorded separately the Pack-AL inference that a learning contract creates a negotiated individual learning context | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.017` as `current-practice`: Knowles's five-part learning contract structures a personal learning process without claiming comparative superiority or guaranteed mastery | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.016` as `current-practice`: Knowles's organizational climate is a condition of learning-process design, not standalone evidence of transfer or work result | Codex |
| 2026-09-11 | Established a mandatory SOTA trace: source-near claim, source boundary, Pack position and owner decision are recorded separately; corpus synthesis and Pack inference cannot be attributed to an individual author | Codex |
| 2026-09-11 | Accepted `STH.KNW.CLAIM.015` as `current-practice`: Knowles's eight process elements form a complete audit map rather than eight mandatory sequential sessions | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.014` as `current-practice`: the adult educator organizes process and resources and helps learning without substituting for the learner's responsibility | Codex |
| 2026-09-11 | Accepted refined `STH.KNW.CLAIM.013` as `bounded`: mutual planning is an andragogical ideal adapted when sponsors specify content or learners cannot yet identify what they need | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.012` as `bounded`: Knowles uses direct or representative learner participation in planning without treating participation as a guarantee of commitment, learning or transfer | Codex |
| 2026-09-11 | Accepted refined `STH.KNW.CLAIM.011` as `current-practice`: diagnostic performance plus feedback may use Knowles's critical incidents, sociodrama, computer games, laboratory exercises or simulations without claiming their comparative superiority | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.010` as `bounded`: practical adult learning is organized around problems, tasks and performance without prohibiting subject-organized study | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.009` as `bounded`: readiness is related to emerging life and work tasks, but an objective task does not establish each learner's recognized readiness | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.008` as `bounded`: Knowles shifts emphasis toward experience-using participatory methods without treating visible activity as proof of learning | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.007` as `bounded`: adult experience can contribute resources and connections while also stabilizing habits and patterns of thought | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.006` as `current-practice`: Knowles's process prepares adults for participation and realistic expectations when they are accustomed to instructor-led learning | Codex |
| 2026-09-11 | Accepted source-near `STH.KNW.CLAIM.005` as `current-practice`: Knowles's three-phase self-diagnosis combines a competence model, diagnostic performance and learner-recognized gap while leaving system justification outside the source claim | Codex |
| 2026-09-11 | Accepted strengthened `STH.KNW.CLAIM.004` as `current-practice`: the learner can inspect the required-action-to-result link, while the source domain owns justification of the action | Codex |
| 2026-09-11 | Accepted `STH.KNW.CLAIM.003` as `current-practice`: learner autonomy and support are set by the person, task, prior capability and situation, not adult age alone | Codex |
| 2026-09-11 | Accepted `STH.KNW.CLAIM.002` as `current-practice`: the six-assumption list is a historical revision, not a closed natural taxonomy | Codex |
| 2026-09-11 | Accepted `STH.KNW.CLAIM.001` as `current-practice`: Knowles's six propositions are testable design assumptions, not universal laws about every adult | Codex |
| 2026-09-11 | Opened `AL.SOTA.028` on Malcolm Knowles's andragogy; registered 20 sources across 12 streams and drafted `STH.KNW.CLAIM.001–026` for owner review without integrating them | Codex |
| 2026-09-09 | Перестроен выбор деятельностных методов по уровням и семействам; стажировка сохранена самостоятельным методом входа в готовую альтернативную систему с обязательным обратным переносом | Codex |
| 2026-09-09 | Normalized applicability conditions for activity-based and developmental methods; added a bounded internship route and the method-selection handoff to Pack-ATB | Codex |
| 2026-09-09 | Clarified the Pack-ATB → Pack-AL capability-demand contract: ATB owns required performers and actions; Pack-AL diagnoses the learning gap, designs learning and returns bounded evidence without redefining the business requirement | Codex |
| 2026-09-09 | Added AL.D.014: separated individual and collective learning from action within current grounds and learning that requires their revision; integrated the distinction into diagnosis, work products, DPF and navigation | Codex |
| 2026-09-08 | Built and internally boundary-tested `AL.P.027 «Организационно-деятельностная игра»` as `candidate/bounded`; kept it outside the selected 24-pattern edition pending real application | Codex |
| 2026-09-08 | Integrated accepted `AL.SOTA.027` claims into existing roles and work products without new entities; OAG-specific team functions and products remain local to future `AL.P.027` | Codex |
| 2026-09-08 | Confirmed working saturation of `AL.SOTA.027` after owner review: six pattern layers and boundary situations are covered by `STH.ODI.CLAIM.001–034`; four evidence deficits remain and constrain `AL.P.027` to `candidate/bounded` | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.034` as bounded: the corpus supports a testable OAG pattern candidate, without claims of comparative superiority, guaranteed effect or safety, or reproducibility from description alone; all 34 claims are now reviewed | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.033` as current practice: OAG classification follows reconstructed method architecture rather than self-label, without treating simpler formats as inferior | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.032` as bounded: reproducibility and safety depend on the whole team's evidenced capabilities, while no validated universal qualification standard was found | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.031` as current practice: emotional intensity and induced pressure are not evidence of development; outcomes and adverse effects are checked independently | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.030` as current practice: known goals, power limits, data use, participation conditions and challenge routes are disclosed to OAG participants | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.029` as bounded: transfer from the temporary OAG system requires a separately designed external transition, whose sufficient architecture is not established by OAG studies | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.028` as current practice and defined activity grounds as a cross-domain Pack synthesis checked through reasoned, self-directed and repeated later action | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.027` as current practice: an OAG product remains a change hypothesis until owned, tried and checked in the external activity system | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.026` as current practice: client outcome and participant development may diverge, so priorities and independent evidence are agreed before the OAG | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.025` as current practice: subject, organizational, learning, research and external results require separate claims and evidence | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.024` as current practice: facilitator influence and content contributions remain explicit, and a fixed answer is not presented as participant co-design | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.023` as bounded: OAG work processes recur through explicit triggers and products rather than following one universal sequence or arbitrary improvisation | Codex |
| 2026-09-08 | Accepted refined `STH.ODI.CLAIM.022` as bounded: self-positioning links a participant to an owned position and action but does not create external authority or prove follow-through | Codex |
| 2026-09-07 | WP-68: extended the RMP ↔ PACK-adult-learning contract to published RMP.3 operationalization and RMP.4 research trace without removing any Pack pattern | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.021` as current practice: a scheme is a contestable means of joint thinking and choosing action, not decoration or methodologist-given truth | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.020` as current practice: reflection reconstructs observable work and informs what to change or retain; changed grounds require evidence in later action | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.019` as bounded: problematizing an established professional way requires material from participants' real activity; work with a case does not prove workplace transformation | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.018` as current practice: problematization exposes an inadequate way and reframes the problem rather than using emotional intensity or devaluing a participant as evidence | Codex |
| 2026-09-07 | Accepted renamed `STH.ODI.CLAIM.017` as bounded: organizing-team functions remain explicit even when roles vary or one person combines several functions | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.016` as bounded: OAG may model future activity while organizing real in-game thought-activity, which does not prove external transfer | Codex |
| 2026-09-07 | Accepted renamed `STH.ODI.CLAIM.015` as current practice: visible group, plenary and reflection forms do not define OAG without functional continuity | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.014` as current practice: the OAG program is a controlled and traceably revised process hypothesis, not a script for participant answers | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.013` as bounded: every classical OAG has a situation-specific organizational design while method invariants remain explicit and reproducible | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.012` as current practice: OAG is estimated across preparation, delivery and exit work without a universal preparation ratio | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.011` as current practice: substantive preparation and diagnosis are part of classical OAG but do not predetermine its content result | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.010` as current practice: OAG composition seeks essential positions, makes absences and proxies explicit, and does not freeze participant positions | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.009` as current practice: system boundaries are explicit, versioned and revisable within the purpose and authority of the work | Codex |
| 2026-09-07 | Accepted `STH.ODI.CLAIM.008` as current practice: order, theme, initial situation and problem-in-game are distinct, with traceable and authorized reframing | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.007` as current practice: OAG organizers may hold hypotheses and govern the process but must preserve openness of the content result | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.006` as bounded: classical OAG addresses a problem not reducible in advance to a known task, while Pack first checks whether a simpler format suffices | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.005` as current practice and synchronized ODI claim summaries: individual, collective-work and external-activity changes require separate evidence | Codex |
| 2026-09-07 | Accepted refined `STH.ODI.CLAIM.004` as bounded: the OAG construction organizes possible collective thought-activity but neither guarantees nor proves its occurrence | Codex |
| 2026-09-06 | Reframed `STH.ODI.CLAIM.003` close to the SMD source and accepted it as bounded; Pack implications remain explicitly separate | Codex |
| 2026-09-06 | Accepted refined `STH.ODI.CLAIM.002` as current practice and separated the SMD claim about two functions of a scheme from the Pack verification rule | Codex |
| 2026-09-06 | Accepted `STH.ODI.CLAIM.001` as bounded: collective thought-activity is a design unit for OAG, not a universal law of cognition | Codex |
| 2026-09-06 | Refined `STH.ODI.CLAIM.001` as a design stance; added two scientific sources distinguishing distributed joint cognition from the stronger SMD ontology | Codex |
| 2026-09-06 | Formulated `STH.ODI.CLAIM.001–034` without a preset cap; owner review pending | Codex |
| 2026-09-06 | Harvested 28 independent works across 12 streams for `AL.SOTA.027`; recorded source independence, coverage, preliminary synthesis and four unresolved evidence gaps | Codex |
| 2026-09-06 | Opened `AL.SOTA.027` for organizational-activity games, thought-activity and the system of thought-activity; source search and claim review pending | Codex |
| 2026-09-05 | Built `AL.P.026 «Лаборатория изменений»` as a candidate/bounded named method from AL.SOTA.026 without adding it to the selected 24-pattern edition | Codex |
| 2026-09-05 | WP-58: implemented the HCD ↔ PACK-adult-learning handoff, narrowed domain ownership and re-evaluated the 24-pattern edition against FPF `d7a7123` | Codex |
| 2026-09-05 | Withdrew `AL.P.025` as a duplicate of Pack-ATB; integrated the educational residue of AL.SOTA.026 into existing routing, developmental and learning-in-transformation entities | Codex |
| 2026-09-04 | Opened AL.SOTA.026 and harvested 23 sources on expansive learning and Change Laboratory, including incomplete interventions and sustainability limits | Codex |
| 2026-09-04 | Built and boundary-tested `AL.P.024 «Интеграция личной и социальной идеологии»`; issued pilot edition `.24` with 24 selected patterns | Codex |
| 2026-09-04 | Built and boundary-tested `AL.P.023 «Коллективное прояснение скрытых условий и отношений власти»`; issued pilot edition `.23` with 23 selected patterns | Codex |
| 2026-09-04 | Built and boundary-tested `AL.P.022 «Рефлексивное участие ради социального изменения»`; issued pilot edition `.22` with 22 selected patterns | Codex |
| 2026-09-04 | Built and boundary-tested `AL.P.021 «Совместное исследование практики»`; issued pilot edition `.21` with 21 selected patterns | Codex |
| 2026-09-03 | WP-56: редакция повторно проверена относительно FPF `0d96c59`; маршрутизатор дополнен выходами в PSD и OCE без изменения выбранного набора из 20 паттернов | Codex |
| 2026-09-02 | WP-54: проверено влияние FPF `3c3f968`; архитектура и выбранный набор сохранены, кандидат `E.23.CAE` отложен до отдельной проверки | Codex |
| 2026-08-31 | Added STH.DEV.069, accepted bounded STH.DEV.CLAIM.044, built and boundary-tested AL.P.020 and issued pilot edition .20 with 20 selected patterns | Codex |
| 2026-08-31 | Reused the released AL.P.019 identifier for the unrelated «Полевые школы» pattern; added ten internal boundary probes and issued pilot edition .19 with 19 selected patterns | Codex |
| 2026-08-30 | WP-49: synchronized the pilot DPF with FPF `72222c13`; clarified performer/Work/assignment and actual temporal structure without changing the selected pattern set | Codex |
| 2026-08-29 | Added STH.DEV.046 and drafted the Action Learning Conversation method passport from the direct five-step workplace procedure by Faller, Marsick and Russell | Codex |
| 2026-08-29 | Reopened AL.SOTA.024 for method harvesting; registered the Mezirow and Associates 1990 collection as a non-counting navigation container and drafted the first method passport on critical incidents | Codex |
| 2026-08-29 | Integrated accepted STH.DEV.CLAIM.031–043 into AL.P.003, AL.P.007–008, AL.P.011, AL.P.013–015, AL.P.017, AL.WP.009, DPF and the domain map; no new roles or work products required | Codex |
| 2026-08-29 | Reopened AL.SOTA.024; added eight primary works by Mezirow and formulated STH.DEV.CLAIM.031–043 on the practical architecture of transformative learning for owner review | Codex |
| 2026-08-29 | Built AL.P.019 as an Argyris–TOC synthesis candidate and tested its boundary against Pack-TOC | Codex |
| 2026-08-29 | Superseded AL.P.019 as a duplicate of Pack-TOC, retained its authoring trace, transferred unique safeguards into five active patterns and issued pilot edition .18 with 18 selected patterns | Codex |
| 2026-08-29 | Expanded AL.SOTA.024 to 33 independent sources and 30 accepted claims with three additional works by Argyris | Codex |
| 2026-08-29 | Separated source class, evidence profile, adoption status and strategic priority; added explicit revision rules and applied them to AL.SOTA.024 | Codex |
| 2026-08-28 | Issued pilot edition .17 with AL.P.018; synchronized DPF-EDITION, README and DPF-PFR for 18 patterns | Codex |
| 2026-08-27 | Reframed the pre-AL.P.009 gate as a cross-Pack router: chronic performance gaps use Pack-ATB; adult-learning receives only the justified action and educational part | Codex |
| 2026-08-24 | Added AL.P.017 for designing a developmental transition; issued pilot edition .16 | Codex |
| 2026-08-24 | Integrated 22 accepted Developmental Andragogy claims as AL.SOTA.024; added AL.D.013, AL.M.009 and AL.WP.009; corrected SoTA count to 24 | Codex |
| 2026-08-23 | Added AL.P.016 for assessing acquired capability with AI; issued pilot edition .15 | Codex |
| 2026-08-23 | Added AL.P.015 for safe questions, warning and closed-loop escalation; issued pilot edition .14 | Codex |
| 2026-08-23 | Added AL.P.014 for problem-, case- and simulation-based learning design; issued pilot edition .13 | Codex |
| 2026-08-23 | Added AL.P.013 for ecosystem design of partner continuing professional education; issued pilot edition .12 | Codex |
| 2026-08-23 | Re-ran 10 boundary probes after AL.SOTA.021 integration; all passed as internal synthetic checks | Codex |
| 2026-08-23 | Integrated STH.ECO.CLAIM.001–010 into existing roles, work products, ecosystem method, distinction, characteristic, failure modes, DPF and map; no new role or work product required | Codex |
| 2026-08-23 | Added AL.P.012 for transforming adult experience into verifiable new action; issued pilot edition .11 | Codex |
| 2026-08-23 | Re-ran 10 boundary probes after AL.SOTA.020 integration; all passed as internal synthetic checks | Codex |
| 2026-08-23 | Integrated STH.EXP.CLAIM.001–010 into experience, reflection, learning-cycle, work-product, distinction and failure-mode guidance | Codex |
| 2026-08-23 | Owner accepted STH.EXP.CLAIM.001–010 with stated statuses and boundaries; integration pending | Codex |
| 2026-08-23 | Formulated STH.EXP.CLAIM.001–010 for owner review in AL.SOTA.020 | Codex |
| 2026-08-23 | Extended AL.SOTA.020 to 26 sources with confidentiality, mandatory reflection and safe-disclosure evidence | Codex |
| 2026-08-23 | Opened AL.SOTA.020 on transforming adult experience into verifiable new action; collected 18 scientific sources | Codex |
| 2026-08-23 | Added AL.P.011 for alignment of learning outcomes, practical tasks and evidence of learning; issued pilot edition .10 | Codex |
| 2026-08-20 | Opened and integrated AL.SOTA.019 on alignment of learning outcomes, practical tasks and evidence of learning; accepted 10 claims from 18 sources | Codex |
| 2026-08-20 | Added AL.P.010 for choosing and revising an individual educational trajectory; issued pilot edition .9 | Codex |
| 2026-08-19 | Integrated AL.SOTA.018 into adaptive trajectory, tutoring, work-product and failure-mode guidance; issued pilot edition .8 | Codex |
| 2026-08-19 | Integrated AL.SOTA.017 into request diagnosis, solution selection, work products and pilot edition .7 | Codex |
| 2026-08-18 | Accepted all claims on measuring incident learning, implementation, sustainability, recurrence, transfer and AI-assisted incident analysis; added AL.SOTA.016 | Codex |
| 2026-08-18 | Accepted claims on worked examples, conditional and reversible fading, component-level criteria, transfer of responsibility and AI support modes; added AL.SOTA.012 | Codex |
| 2026-08-18 | Accepted all claims on productive help-seeking, avoidance, premature hints, source choice, escalation and AI answer substitution; added AL.SOTA.013 | Codex |
| 2026-08-18 | Accepted all claims on psychological safety, leader response, warning signals, closed-loop escalation and the hypothetical AI first-contact channel; added AL.SOTA.014 | Codex |
| 2026-08-18 | Accepted all claims on error learning, incident review, fair accountability, just culture boundaries and automation bias; added AL.D.012 and AL.SOTA.015 | Codex |
| 2026-08-18 | Accepted evidence-based claims on retrieval practice, retention, corrective attempts and boundaries of transfer; added AL.SOTA.010 | Codex |
| 2026-08-17 | Accepted evidence-based claims on feedback effects, goal alignment and next-action use; added AL.SOTA.009 | Codex |
| 2026-08-17 | Accepted evidence-based claims on workplace transfer, work-environment conditions and transfer measurement; added AL.SOTA.008 | Codex |
| 2026-08-16 | Added evidence-based distinction between AI-supported performance and acquired capability; refined AI SoTA | Codex |
| 2026-07-28 | Initial DPF/Pack built from local source corpus | Codex |
