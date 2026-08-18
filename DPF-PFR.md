# DPF-PFR

## 1. Назначение

Файл содержит только отношения и записи, для которых существует конкретная задача сопровождения пилотной редакции `DPF-EDITION@pilot-2026-08-18`.

Идентификатор, строка или соседство записей не создают отношение. Сначала формулируется прямое предметное утверждение; обслуживающая запись представляет его для проверки влияния обновления.

## 2. Прямая зависимость от FPF

`DPF-EDITION@pilot-2026-08-18` использует правила авторинга, видов, отношений, качества и пакетной оценки из FPF Левенчука в коммите `3d098629dc218572089f1890080c17d6f1d9a867` как необходимые ограничения для пилотного DPF-авторинга и проверки.

Без этих правил либо после их содержательно значимого изменения утверждения о соответствии `E.8`, результатах `E.21`, границах предметных видов и пакетной оценке не могут оставаться текущими без повторной проверки. Поэтому пилотная редакция зависит от указанного содержания точной редакции FPF для авторинга и оценки.

FPF Core не зависит от этой редакции. Совместимость сверх названного использования не заявляется.

## 3. FrameworkEditionDependencyRecord

```yaml
FrameworkEditionDependencyRecord@DPF-EDITION-pilot-2026-08-18:
  subjectAssertionRef: DPF-PFR:2
  dependencyPredicateClaimRef: E.4.PFR:3.4-framework-edition-dependency-predicate
  directionConstraintClaimRef: E.5.3-domain-to-Core-direction-and-Core-acyclicity
  dependentEditionRef: DPF-EDITION@pilot-2026-08-18
  reliedOnEditionRef: FPF@3d098629dc218572089f1890080c17d6f1d9a867
  reliedOnContentRefs:
    - E.4.DPF
    - E.4.PFAD
    - E.4.PFR
    - E.4.DPF.DA
    - E.8
    - E.9
    - E.21
    - E.24.PUB
  namedUse: DPF authoring, pattern evaluation and package evaluation
  dependencyDirection: domain_DPF_to_FPF_Core
  dependencyReason: a relevant change to selected Core rules invalidates or reopens affected authoring and evaluation claims
  refreshConditionRefs:
    - DPF-EDITION:9-FPF-change-trigger
  compatibilityClaimRefs: []
```

Эта запись зеркалирует прямое утверждение раздела 2. Она не доказывает зависимость, совместимость, выполненную проверку или актуальность сама по себе.

## 4. Прямые отношения пилотных паттернов

`AL.P.001` и `AL.P.002` являются соседними самостоятельными паттернами одного пилотного выбранного набора. Обязательный порядок между ними не установлен.

`AL.P.002` рекомендует обратиться к `AL.P.001` только когда после помощи заявлено научение, устойчивость или перенос, для которых нужна отдельная проверка. Эта рекомендация не утверждает, что помощь была оказана, научение состоялось или применение второго паттерна обязательно.

Отдельный `PatternFrameworkRelationRecord` для этих утверждений не создаётся: текущая навигация обслуживается телами паттернов и README, а независимая задача межпаттернового индекса или сравнения не заявлена.

## 5. Граница редакций

Положительное `EpistemeEditionRelation` с прежним состоянием Pack не заявляется. Предыдущее состояние было авторским репозиторием и прототипом, но его идентичность как точной редакции DPF не была установлена.

Git-история сохраняет происхождение файлов, но сама по себе не доказывает тождество эпистем, продолжение редакции, совместимость или замещение. Эти отношения могут быть заявлены позже только при наличии отдельной задачи и достаточного основания.

## 6. Публикация и доступ

Публикационный результат не заявляется. `README.md` и выбранные файлы образуют подготовленный читательский набор для локальной проверки, но следующие утверждения пока отсутствуют:

- отдельное публикационное событие;
- утверждённое публичное предметное название;
- декларация публичной аудитории;
- установленное отношение формы и точной редакции;
- установленное отношение носителя и формы;
- подтверждённая непрерывная доступность для объявленной аудитории.

Следовательно, `EpistemePublicationRelation` и внешний access relation не утверждаются. Наличие файлов в Git не заполняет эти пропуски.

## 7. FrameworkPackageManifest

```yaml
FrameworkPackageManifest@DPF-EDITION-pilot-2026-08-18:
  frameworkEditionRef: DPF-EDITION@pilot-2026-08-18
  selectedPatternSetResultRef: DPF-EDITION:3
  relationRecordRefs: []
  dependencyAndEditionRecordRefs:
    - FrameworkEditionDependencyRecord@DPF-EDITION-pilot-2026-08-18
  editionStatus: admissibleForDeclaredDPFUse
  deprecationOrSupersessionRefs: []
  sourcePackRefs:
    - 06-sota/source-register.md
  qualityEvidenceRefs:
    - РП Миграция PACK-adult-learning с SPF на DPF FPF.md:10.1
    - РП Миграция PACK-adult-learning с SPF на DPF FPF.md:11.2
    - РП Миграция PACK-adult-learning с SPF на DPF FPF.md:13
    - РП Миграция PACK-adult-learning с SPF на DPF FPF.md:16
    - РП Миграция PACK-adult-learning с SPF на DPF FPF.md:17
  refreshPlanOrCurrentnessRefs:
    - DPF-EDITION:9
  firstEntryCarrierRefs:
    - README.md
  blockedRuntimeOrBuildReading: this index creates no runtime dependency, file membership, publication, access, Work, authority or evidence relation
```

Манифест индексирует обслуживаемые ссылки для проверки редакции. Он не является редакцией, выбранным набором, публикацией или доказательством содержащихся утверждений.
