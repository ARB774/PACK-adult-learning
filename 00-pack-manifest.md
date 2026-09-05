# Pack Manifest: Adult Learning and Continuing Professional Education
## Metadata
```yaml
pack_id: AL
pack_name: Проектирование обучения взрослых и программ ДПО
pack_name_en: Adult Learning and Continuing Professional Education Design
version: 0.1.0
fpf_edition: 0d96c59d9795bf742f2100be847dc2d68851b87a
fpf_edition_date: 2026-09-03
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
last_updated: 2026-09-04
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
## Object of description
Объект описания — воспроизводимая практика проектирования, проведения, сопровождения и оценки обучения взрослых, создающая наблюдаемые изменения в способности действовать и применять результат в профессиональном или жизненном контексте.
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
| Pack-ATB | При признанном хроническом разрыве результативности предоставляет системную диагностику и разработанное решение; Pack-adult-learning принимает обоснованное изменение действий и проектирует только образовательную часть. Если АТБ неприменима, происхождение основания и маршрут фиксируются явно. |
| Pack-TOC | `AL.P.001`, `AL.P.008`, `AL.P.012`, `AL.P.015` и прежде всего `AL.P.017` не выявляют ограничивающее убеждение собственным методом. Они передают наблюдаемое расхождение и обе стороны конфликта в Pack-TOC: `TOC.M.003` строит полную тучу, `TOC.M.004` опознаёт кандидата в ограничивающее предположение, `TOC.M.009` проверяет конфликт заявленной и фактической линии действия, а `TOC.D.006` отделяет предположение от элемента тучи. Точная опора: коммит `44c876e1f58b50e61b2625a927890a3791b99532`. |
| PSD DPF | Получает запрос, когда до образовательной диагностики нужно удержать несколько формулировок проблемы, участников, ценности, альтернативы и неопределённость и подготовить рекомендацию владельцу выбора. Рекомендация не создаёт решение или мандат. |
| OCE DPF | Получает обоснованную неучебную часть, когда рабочая проба требует изменить роли, полномочия, отношения вкладов или устройство продолжающейся работы. План переноса не заменяет инженерное получение организации. |
## Content summary
| Section | Count | Status |
|---|---:|---|
| Distinctions | 13 | draft |
| Roles | 7 | draft |
| Objects of attention | 10 | draft |
| Methods | 10 | draft |
| Work products | 10 | draft |
| Failure modes | 10 | draft |
| Characteristics | 8 | draft |
| SoTA annotations/source groups | 26 | draft |
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
