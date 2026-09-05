---
id: AL.MAP.001
name: Карта проектирования обучения взрослых
scope: full-pack
summary: Навигация от запроса взрослого через учебный опыт к переносу и доказательству эффекта.
created: 2026-07-28
last_updated: 2026-08-29
generated: false
---

# [AL.MAP.001] Карта домена

## Core flow

```mermaid
flowchart LR
    A["Исходный запрос и контекст системы"] --> M10["AL.M.010 Выбор маршрута"]
    M10 --> W10["WP.010 Основание и маршрут"]
    W10 -->|образовательная часть подтверждена| M1["AL.M.001 Диагностика запроса"]
    W10 -->|хронический разрыв результативности| ATB["Pack-АТБ"]
    ATB -->|образовательная часть системного решения| M1
    M1 --> W1["WP.001 Профиль запроса"]
    M1 --> W2["WP.002 Карта результатов"]
    W1 --> M4["M.004 Самонаправленность"]
    W1 --> M5["M.005 Тьюторство"]
    W2 --> M2["M.002 Опыт — осмысление — действие"]
    M2 --> W3["WP.003 Архитектура опыта"]
    M2 --> W4["WP.004 Практическое задание"]
    W4 --> M3["M.003 Проблемно-кейсовое обучение"]
    M3 --> W5["WP.005 Критериальная шкала и доказательства"]
    W4 --> M6["M.006 Перенос"]
    M6 --> W7["WP.007 План переноса"]
    W5 --> M7["M.007 Оценивание эффектов"]
    W7 --> M7
    M7 --> W8["WP.008 Отчёт об эффектах"]
    M8["M.008 Экосистемное ДПО"] -. согласует .-> W2
    M8 -. обеспечивает среду .-> W7
    W2 --> M9["M.009 Развивающий переход"]
    M2 -. конфликт и данные .-> TOC9["Pack-TOC: полная туча и ограничивающее предположение"]
    TOC9 -. проверенное основание .-> M9
    M9 --> W9["WP.009 Карта развивающего перехода"]
    W9 --> M6
    W9 --> M7
```

## Navigation

| Need | Start | Then |
|---|---|---|
| Понять границы домена | `01A-bounded-context.md` | `ontology.md` |
| Не путать ключевые понятия | `01B-distinctions.md` | `05-failure-modes/failure-modes.md` |
| Спроектировать обратную связь | AL.P.003 (`pilot`) | AL.D.006, AL.SOTA.009, AL.M.002, AL.WP.004, AL.WP.005 |
| Спроектировать воспроизведение по памяти | AL.P.004 (`pilot`) | AL.D.004, AL.D.006, AL.SOTA.010, AL.M.002, AL.M.003, AL.WP.003–005 |
| Управлять когнитивными требованиями и поддержкой | AL.P.005 (`pilot`) | AL.D.004, AL.D.011, AL.SOTA.011, AL.M.002–004, AL.WP.003, AL.WP.004, AL.WP.006 |
| Перевести от примера к самостоятельному действию | AL.P.005 (`pilot`) | AL.D.004, AL.D.011, AL.SOTA.012, AL.M.002, AL.M.004, AL.WP.003, AL.WP.004, AL.WP.006 |
| Спроектировать продуктивный запрос помощи | AL.P.002 (`pilot`) | AL.OA.007, AL.D.006, AL.SOTA.013–014, AL.M.002, AL.M.004, AL.M.005, AL.WP.003, AL.WP.006 |
| Обеспечить безопасный вопрос, предупреждение и эскалацию | AL.P.015 (`pilot`) | AL.SOTA.014, AL.OA.007, AL.R.003–005, AL.M.004–005, AL.WP.006, AL.FM.008 |
| Учиться на ошибке и справедливо распределять ответственность | AL.P.006 (`pilot`) | AL.D.012, AL.SOTA.015, AL.M.002, AL.M.004, AL.WP.005, AL.WP.006, AL.FM.005, AL.FM.008 |
| Доказать научение из ошибки или инцидента | AL.P.001 (`pilot`) | AL.D.007, AL.SOTA.016, AL.M.006, AL.M.007, AL.WP.005, AL.WP.007, AL.WP.008, AL.FM.006, AL.FM.007 |
| Проверить освоенную способность при использовании ИИ | AL.P.016 (`pilot`) | AL.SOTA.023, AL.D.011, AL.R.001–003, AL.R.005, AL.R.007, AL.WP.002, AL.WP.004–005, AL.WP.008 |
| Проверить основание запроса и выбрать системный маршрут | AL.P.018 (`pilot`) | AL.SOTA.025, AL.M.010 → AL.WP.010 → Pack-АТБ, другой системный домен, прямая проверка или остановка |
| Проверить образовательную часть и выбрать тип решения | AL.P.009 (`pilot`) | после AL.WP.010: AL.D.003, AL.SOTA.017, AL.M.001 → AL.WP.001; при подтверждённой образовательной части → AL.WP.002 |
| Согласовать результат, практическое задание и доказательство освоения | AL.P.011 (`pilot`) | AL.SOTA.019, AL.WP.002–005, AL.M.002, AL.M.003, AL.M.007 |
| Спроектировать учебный кейс, проблему или симуляцию | AL.P.014 (`pilot`) | AL.SOTA.022, AL.M.003, AL.R.002–003, AL.R.005 → AL.WP.003–005 |
| Преобразовать профессиональный опыт в проверяемое новое действие | AL.P.012 (`pilot`) | AL.SOTA.020, AL.OA.002, AL.OA.006, AL.M.002 → AL.WP.003 |
| Выявить конфликт и ограничивающее убеждение для развивающего перехода | Pack-TOC `TOC.M.003`, `TOC.M.004`, `TOC.M.009`, `TOC.D.006` | проверить обе стороны конфликта и передать результат в AL.P.017 → AL.WP.009 |
| Выбрать и пересматривать индивидуальную траекторию | AL.P.010 (`pilot`) | AL.D.009, AL.M.004, AL.M.005, AL.SOTA.018 → AL.WP.006 |
| Обеспечить рабочее применение | AL.P.007 (`pilot`) | AL.M.006, AL.SOTA.008, AL.WP.007, AL.WP.008 |
| Оценить эффект | AL.P.008 (`pilot`) | AL.M.007, AL.WP.005, AL.WP.008 |
| Построить партнёрскую ДПО | AL.P.013 (`pilot`) | AL.SOTA.021, AL.M.008, AL.R.001–002, AL.R.004–007 → AL.WP.002, AL.WP.007, AL.WP.008 |
| Спроектировать развивающий переход | AL.P.017 (`pilot`) | AL.SOTA.024, AL.D.013, AL.M.009, AL.R.001–003, AL.R.005–007 → AL.WP.009 → AL.WP.003–005, AL.WP.007–008 |
| Проверить новое основание в реальной совместной работе до масштабирования | AL.P.019 (`pilot`) | AL.SOTA.024, Pack-TOC, AL.P.017, AL.M.009 → AL.WP.009 → AL.P.003, AL.P.007–008 |
| Освоить действие на новом основании в обычной рабочей среде | AL.P.020 (`pilot`) | AL.SOTA.024, STH.DEV.069, AL.P.017, AL.M.009 → AL.WP.009 → AL.P.003, AL.P.005, AL.P.007–008; при блокировке среды → AL.P.019 |
| Построить ещё неизвестное решение совместно с группой практиков | AL.P.021 (`pilot`) | AL.SOTA.024, STH.DEV.042, STH.DEV.058–060, AL.M.002 → AL.WP.003, AL.WP.007–009 → AL.P.003, AL.P.007–008, AL.P.012–013, AL.P.015, AL.P.017, AL.P.019–020 |
| Встроить научение в уже принадлежащее группе организационное изменение | AL.P.022 (`pilot`) | AL.SOTA.024, STH.DEV.045, STH.DEV.062, AL.M.002, AL.M.009 → AL.WP.003, AL.WP.007–009 → AL.P.003, AL.P.007–008, AL.P.012, AL.P.015, AL.P.017–021 |
| Проверить, не создаёт ли повторяющееся «личное» затруднение сама система | AL.P.023 (`pilot`) | AL.SOTA.024, STH.DEV.045, STH.DEV.061, AL.P.018, AL.M.010 → AL.WP.010 → AL.P.009, AL.P.012, AL.P.015, AL.P.017, AL.P.021–022, Pack-АТБ, Pack-TOC |
| Связать основание конкретного человека с поддерживающими условиями организации и выбрать предмет изменения | AL.P.024 (`pilot`) | AL.SOTA.024, STH.DEV.045, STH.DEV.063–064, AL.P.018, AL.M.009 → AL.WP.009 → AL.P.009, AL.P.012, AL.P.017, AL.P.019–020, AL.P.023, Pack-АТБ, Pack-TOC |
| Организовать научение группы внутри обоснованной и полномочной трансформации | AL.P.022 (`pilot`) | Pack-АТБ или другой предметный домен → AL.P.018 → AL.SOTA.026, AL.M.009 → AL.WP.009 → AL.P.020, AL.P.007–008; AL.P.025 отозван как междоменный дубль |
| Проверить основание, статус и границы утверждения | `06-sota/source-register.md` | профиль оснований, допустимое использование и критерий пересмотра |

## Quality gates

1. **Routing gate:** WP.010 фиксирует происхождение запроса, границу рассматриваемой системы, первое лицо, мандат, тип ситуации и маршрут; хронический разрыв результативности не подменяется локальной диагностикой обучения.
2. **Request gate:** WP.001 содержит действие, контекст и авторство цели, принятые из зафиксированного маршрута.
3. **Alignment gate:** результат, практика и доказательство связаны моделями способности, доказательства и задания; уровень действия, выборка задач, режим поддержки, индивидуальность вывода и последствия решения названы.
4. **Adult-learning gate:** опыт и готовность к самостоятельности реально диагностированы.
5. **Safety gate:** проблематизация, обратная связь и сбор данных имеют границы и право отказа; комментарий о личности не подменяет данные о задаче, процессе и саморегуляции.
6. **Transfer gate:** среда применения и ответственность сторон подтверждены, а вывод о переносе опирается не только на самоотчёт и учитывает тип рабочего действия.
7. **Evidence gate:** сила вывода не превышает качество данных.
8. **AI-support gate:** названы объект вывода, целевой режим и существенные действия человека; результат сеанса, способность человека и способность системы «человек + ИИ» не смешаны; контроль проверен на полезной и существенно ошибочной рекомендации; происхождение опирается на совокупность свидетельств; изменение, сбой и граница конфигурации соответствуют широте вывода; поддержанное выполнение, освоение и эффект программы разделены.
9. **Retention gate:** если требуется долговременное сохранение знания, архитектура включает воспроизведение без доступа к образцу, коррекцию ошибки и новую попытку; перенос в рабочую практику проверяется отдельно.
10. **Cognitive-demands gate:** существенная сложность, лишние требования, реалистичность и временная поддержка различены; самостоятельная способность не выводится только из выполнения с подсказкой.
11. **Support-transfer gate:** помощь соответствует конкретному выполнению, допускает снятие и возврат, а передача ответственности подтверждается самостоятельной контрольной пробой.
12. **Help-seeking gate:** для затруднения заданы доступные источники, минимально достаточные уровни помощи и условия немедленной эскалации; после помощи участник перерабатывает ответ и выполняет новую пробу, а качество не выводится из числа вопросов.
13. **Psychological-safety gate:** реальная реакция на вопрос, ошибку и предупреждение не унижает добросовестного участника; для угрозы заданы адресат с полномочиями, срок подтверждения, следующий уровень и возврат результата, а предметные стандарты и ответственность сохранены.
    Регистрация не считается закрытием; режим канала и предел идентифицируемости объявлены; при конфликте доступен независимый адресат; число сообщений не заменяет данные реакции и результата; цифровой или ИИ-вход подтверждает передачу человеку с полномочиями.
14. **Error-learning gate:** действие, исход, нарушение и вывод об ответственности различены; защищённая учебная ошибка ведёт к коррекции и новой пробе, а рабочее событие — к сохранению данных, проверяемому изменению и объяснимому решению по объявленной процедуре.
15. **Incident-learning evidence gate:** сообщение, вывод, изменение, внедрение, соблюдение, результат, устойчивость и перенос измеряются раздельно; число сообщений и закрытых мероприятий не подменяют операционный эффект, а показатели учитывают экспозицию и ограничения интерпретации.
16. **Request-diagnosis gate:** тема и разрыв выполнения не выданы за образовательную потребность; целевое действие установлено, а способность, возможность и мотивация проверены по достаточным данным.
17. **Adaptive-trajectory gate:** назван изменяемый компонент, данные, правило, ожидаемый результат и контрольная точка; активность сопровождения и ИИ-рекомендация не выданы за результат.
18. **Experience-transformation gate:** след события отделён от позднего объяснения; стаж не выдан за экспертизу; есть проверяемая альтернатива и изменённая проба; функции раскрытия, читатели, последствия и предел конфиденциальности известны.
19. **Partner-configuration gate:** каждый партнёр закрывает необходимый переход; результаты сторон, локальные обязательства, рабочий объект, критерий приёмки, полномочия, данные и сценарий отказа названы; процесс сети не выдан за результат взрослого, а ИИ не назначен владельцем решения.
20. **Problem-case gate:** вид конструкции назван по действию и реакции среды; существенные признаки меняют решение; информационный режим и поддержка функциональны; совместный продукт имеет индивидуальный след; разбор ведёт к новой пробе; выборка, симуляция и ИИ имеют явные границы вывода.
21. **Development gate:** освоение, совершенствование и развитие различены, выбрана минимально достаточная глубина; содержание, способ решения и предпосылки не смешаны; противоречие не создаётся искусственным потрясением; проверяемый диалог допускает данные, возражения и альтернативы; новое объяснение доведено до плана, способности, безопасной пробы и повтора; названы авторство, мандат, поддержка и препятствия среды, «Я — Мы — Это», жизнеспособность и раздельные непосредственный, отсроченный и организационный результаты. Если основание связано с устойчивым конфликтом, обе стороны проверены средствами Pack-TOC без предположения о заранее неправом исполнителе; гипотеза открыта для исправления.
22. **Field-school gate:** проверенное решение испытывается на ограниченном реальном объекте во временно разрешённой системе ролей и правил; выполнены повторные циклы с данными; самостоятельность, перенос и эффект всей системы проверяются отдельно от группового согласия и локального результата.
23. **Action-research gate:** принятие новой перспективы не выдано за способность; опорная модель конкретна и пересматриваема; участник сохраняет существенные решения; реальные циклы меняются по данным; поддержка снимается; препятствия основания, модели, способности и среды разделены.
24. **Collaborative-inquiry gate:** вопрос действительно принадлежит группе и не имеет назначенного ответа; полномочия и должностная власть видимы; конкурирующие объяснения проверяются повторными рабочими циклами; отрицательные случаи и особые мнения сохраняются; предварительное знание ограничено проверенными условиями; индивидуальное научение, групповая практика и системный эффект разведены.
25. **Reflective-participation gate:** устойчивая группа действительно владеет ведущимся изменением; участие не скрывает чужого решения или риска санкций; цель и локальный интерес проверены относительно целой системы; завершённый эпизод ведёт к отличающемуся следующему действию; преподаватель не присваивает управление; индивидуальное научение, совместная способность, ход изменения и системный эффект разведены.
26. **Collective-clarification gate:** несколько сопоставимых эпизодов людей в сходном положении отделены от оценок; первый круг защищён от прямой санкционной зависимости; повторяющиеся условия сопоставлены с исключениями; личные и системные объяснения сохранены; отношения власти не назначены причиной заранее; гипотеза ограничена и передана владельцу или в предметный домен.
27. **Personal-social-integration gate:** конкретный эпизод связан с личным основанием, его прежней полезностью и необходимой функцией; организационное условие проверено отдельно; человек и система не назначены причиной заранее; выбран предмет изменения; новое действие и изменение условия согласованы по владельцам, мандату, риску и раздельным результатам.
28. **Learning-within-transformation gate:** происхождение, решение и организационная часть преобразования получены из Pack-АТБ, OCE или другого компетентного домена; заданное отделено от решений группы; наблюдаемые данные отделены от диагноза консультанта; есть мандат, безопасное возражение, рабочая проба и повтор; индивидуальное освоение, совместная способность, практика, устойчивость и системный эффект имеют отдельные свидетельства.

## Update log

| Date | Change |
|---|---|
| 2026-09-05 | Withdrew AL.P.025 as a cross-domain duplicate of Pack-ATB; integrated the educational residue of AL.SOTA.026 into AL.P.018, AL.P.017, AL.P.020, AL.P.022, AL.M.009 and AL.WP.009 |
| 2026-09-04 | Opened AL.SOTA.026 and added navigation to the 23-source corpus on expansive learning and Change Laboratory |
| 2026-09-04 | Added AL.P.024 for linking a person's basis with organizational conditions and choosing a coordinated object of change |
| 2026-09-04 | Added AL.P.023 for testing whether repeated individual difficulties are reproduced by shared organizational conditions and power relations |
| 2026-09-04 | Added AL.P.022 for learning inside a real change already owned by a stable group, with explicit protection against pseudo-participation |
| 2026-09-04 | Added AL.P.021 for jointly owned cycles that build provisional contextual knowledge when no reliable solution is ready |
| 2026-08-31 | Added AL.P.020 for repeated real-work action research with a provisional practice model and fading support |
| 2026-08-31 | Added AL.P.019 «Полевые школы» as a bounded temporary activity-system pattern and separated it from seminars, simulations and ordinary pilots |
| 2026-08-29 | Reopened AL.SOTA.024 to harvest reproducible transformative-learning methods while preserving each chapter author's attribution |
| 2026-08-29 | Integrated STH.DEV.CLAIM.031–043 into the development route and related feedback, transfer, evidence, partnership, case and safety patterns; no new entities required |
| 2026-08-29 | Reopened AL.SOTA.024 with eight primary works by Mezirow and 13 proposed claims on levels of change, discourse, reflection, support, provisional roles and reintegration; pattern integration awaits owner review |
| 2026-08-29 | Superseded the duplicate AL.P.019 candidate; routed conflict and limiting-assumption work directly through Pack-TOC and retained its unique safeguards in active patterns |
| 2026-08-29 | Built and boundary-tested AL.P.019 as a candidate before deciding domain ownership |
| 2026-08-29 | Expanded AL.SOTA.024 with the explicit 1974–1996 Argyris and Schön source line |
| 2026-08-29 | Added navigation to the multi-channel evidence profile, adoption status and revision criterion |
| 2026-08-27 | Added AL.P.018, AL.M.010 and AL.WP.010 as the cross-Pack request router before AL.P.009; chronic performance gaps route through Pack-ATB |
| 2026-08-24 | Added AL.P.017 as the entry for designing a developmental transition |
| 2026-08-24 | Integrated AL.SOTA.024; added navigation for AL.D.013, AL.M.009, AL.WP.009 and the development gate |
| 2026-08-23 | Added navigation for full `AL.P.016` and included it in the sixteen-pattern pilot edition |
| 2026-08-23 | Integrated `STH.AIC.CLAIM.001–010`: expanded AI-supported capability distinction, roles, evidence products, failure modes and AI-support gate; no new roles or work products required |
| 2026-08-23 | Added AL.P.015 as the entry for safe questions, warning and closed-loop escalation |
| 2026-08-23 | Integrated reopened AL.SOTA.014 supplements into escalation guidance and added AL.P.015 candidate navigation |
| 2026-08-23 | Added AL.P.014 as the entry for problem-, case- and simulation-based learning design |
| 2026-08-23 | Integrated accepted AL.SOTA.022 claims and working definitions into problem/case method, roles, work products, distinctions, failure modes and DPF guidance |
| 2026-08-23 | Added AL.P.013 as the entry for ecosystem design of partner continuing professional education |
| 2026-08-23 | Integrated accepted AL.SOTA.021 claims into ecosystem method, roles, work products, distinctions, failure modes and DPF guidance |
| 2026-08-23 | Added AL.P.012 as the entry for transforming adult experience into verifiable new action |
| 2026-08-23 | Integrated AL.SOTA.020 into experience, reflection, learning-cycle, work-product, distinction and failure-mode guidance |
| 2026-08-23 | Added AL.P.011 as the entry for alignment of learning outcomes, practical tasks and evidence of learning |
| 2026-08-20 | Opened and integrated AL.SOTA.019 for alignment of outcomes, practical tasks and evidence of learning |
| 2026-08-20 | Added AL.P.010 as the entry for choosing and revising an individual educational trajectory |
| 2026-08-18 | Integrated AL.SOTA.016 into incident-learning measurement, implementation evidence, sustainability and transfer |
| 2026-08-19 | Integrated AL.SOTA.017 into request diagnosis, solution selection and evidence products |
| 2026-08-19 | Integrated AL.SOTA.018 into adaptive trajectory, tutoring, work-product and failure-mode guidance |
| 2026-08-18 | Integrated AL.SOTA.012 into example-to-action transition, adaptive support and AI target modes |
| 2026-08-18 | Integrated AL.SOTA.013 into self-regulation, tutoring, help-source selection, escalation and AI-help modes |
| 2026-08-18 | Integrated AL.SOTA.014 into psychological safety, response to questions, safety voice and closed-loop escalation |
| 2026-08-18 | Integrated AL.SOTA.015 into error distinctions, protected practice, incident learning and fair accountability |
| 2026-08-18 | Integrated AL.SOTA.011 into learning-cycle, case, adaptive-support and cognitive-demands navigation |
| 2026-08-18 | Integrated AL.SOTA.010 into learning-cycle, task, evidence and retention navigation |
| 2026-08-17 | Integrated AL.SOTA.009 into feedback navigation and safety gate |
| 2026-08-17 | Integrated AL.SOTA.008 into transfer navigation and evidence gate |
| 2026-08-16 | Added navigation and quality gate for AL.D.011; linked AL.SOTA.006 to evidence products |

