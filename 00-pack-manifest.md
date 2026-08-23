# Pack Manifest: Adult Learning and Continuing Professional Education

## Metadata

```yaml
pack_id: AL
pack_name: Проектирование обучения взрослых и программ ДПО
pack_name_en: Adult Learning and Continuing Professional Education Design
version: 0.1.0
fpf_edition: 3d098629dc218572089f1890080c17d6f1d9a867
fpf_edition_date: 2026-08-16
architecture_decision: DPF-DRR.md
pilot_edition_ref: DPF-EDITION@pilot-2026-08-23.14
pilot_edition_record: DPF-EDITION.md
relation_maintenance_record: DPF-PFR.md
pilot_selected_patterns: [AL.P.001, AL.P.002, AL.P.003, AL.P.004, AL.P.005, AL.P.006, AL.P.007, AL.P.008, AL.P.009, AL.P.010, AL.P.011, AL.P.012, AL.P.013, AL.P.014, AL.P.015]
public_name: not_selected
publication_occurrence: not_asserted
pilot_evaluation_status: admissibleForDeclaredDPFUse
pilot_evaluation_floor: 3
spf_template_checked: 2026-07-28
status: draft
created: 2026-07-28
last_updated: 2026-08-20
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

## Content summary

| Section | Count | Status |
|---|---:|---|
| Distinctions | 12 | draft |
| Roles | 7 | draft |
| Objects of attention | 9 | draft |
| Methods | 8 | draft |
| Work products | 8 | draft |
| Failure modes | 10 | draft |
| Characteristics | 7 | draft |
| SoTA annotations/source groups | 20 | draft |
| Maps | 1 | draft |

## Entity index

| ID | Name | Kind | Summary | Status |
|---|---|---|---|---|
| AL.M.001 | Диагностика образовательного запроса | M | Связывает цели взрослого, контекст труда, опыт, ограничения и требуемый результат | draft |
| AL.M.002 | Проектирование цикла «опыт — осмысление — действие» | M | Превращает опыт и практическое действие в переносимое знание | draft |
| AL.M.003 | Проблемно-кейсовое обучение | M | Организует освоение через реалистичную проблему или кейс | draft |
| AL.M.004 | Поддержка самонаправленного обучения | M | Настраивает объём выбора и опоры по готовности обучающегося | draft |
| AL.M.005 | Тьюторское сопровождение траектории | M | Помогает удерживать запрос, рефлексию и следующий карьерно-образовательный шаг | draft |
| AL.M.006 | Проектирование переноса в рабочую практику | M | Встраивает применение, поддержку и проверку результата после обучения | draft |
| AL.M.007 | Оценивание эффектов обучения | M | Собирает доказательства обучения, поведения и контекстных результатов | draft |
| AL.M.008 | Экосистемное проектирование ДПО | M | Связывает необходимые вклады сторон, проверяемые переходы, полномочия, данные и устойчивость конфигурации | draft |
| AL.WP.001 | Профиль образовательного запроса | WP | Проверяемое описание цели, опыта, контекста и ограничений | draft |
| AL.WP.002 | Карта результатов и компетенций | WP | Связывает действия, критерии и доказательства освоения | draft |
| AL.WP.003 | Архитектура учебного опыта | WP | Отображает последовательность опыта, рефлексии, концептуализации и действия | draft |
| AL.WP.004 | Практическое задание | WP | Задание, имитирующее или выполняющее реальную деятельность | draft |
| AL.WP.005 | Критериальная шкала оценки и план доказательств | WP | Фиксирует критерии качества и допустимые свидетельства | draft |
| AL.WP.006 | План индивидуальной траектории и сопровождения | WP | Описывает выбор, опоры, контрольные точки и пересмотр маршрута | draft |
| AL.WP.007 | План переноса в рабочую практику | WP | Фиксирует применение, среду, поддержку и проверку после обучения | draft |
| AL.WP.008 | Отчёт об эффектах | WP | Сводит данные об участии, освоении, поведении и результатах контекста | draft |

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
| 2026-08-18 | Accepted claims on cognitive load, worked examples, fading support, coherent presentation and supported-performance boundaries; added AL.SOTA.011 | Codex |
| 2026-08-18 | Accepted evidence-based claims on retrieval practice, retention, corrective attempts and boundaries of transfer; added AL.SOTA.010 | Codex |
| 2026-08-17 | Accepted evidence-based claims on feedback effects, goal alignment and next-action use; added AL.SOTA.009 | Codex |
| 2026-08-17 | Accepted evidence-based claims on workplace transfer, work-environment conditions and transfer measurement; added AL.SOTA.008 | Codex |
| 2026-08-16 | Added evidence-based distinction between AI-supported performance and acquired capability; refined AI SoTA | Codex |
| 2026-07-28 | Initial DPF/Pack built from local source corpus | Codex |

