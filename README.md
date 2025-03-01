# Cheatsheets (Шпаргалки)
<!--
https://backendinterview.ru/index.html
-->

## Парадигмы
<!--
https://ru.wikipedia.org/wiki/%D0%9F%D0%B0%D1%80%D0%B0%D0%B4%D0%B8%D0%B3%D0%BC%D0%B0_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F
-->
### Основные модели
- Императивное программирование
- Декларативное программирование
- Структурное программирование
- Функциональное программирование
- Логическое программирование
- Объектно-ориентированное программирование (ООП)
  - Компонентно-ориентированное программирование
  - Прототипно-ориентированное программирование
  - Агентно-ориентированное программирование

### Подходы и приёмы
- Структурное программирование
- Процедурное программирование
- Аппликативное программирование
- Обобщённое программирование
- Доказательное программирование
- Порождающее программирование
- Аспектно-ориентированное программирование (АОП)
- Агентно-ориентированное программирование
- Контрактное программирование
- Рекурсия
- Автоматное программирование
- Событийно-ориентированное программирование
- Компонентно-ориентированное программирование
- Грамотное программирование

## Концепции
- [Принцип DRY](concepts/dry.md)
- [Принципы KISS](concepts/kiss.md)
- [Принципы SOLID](concepts/solid.md)
- [Принципы YAGNI](concepts/yagni.md)
- [Паттерны GRASP](concepts/grasp.md)
- [Паттерны GoF](concepts/gof.md)
- [Требования ACID](concepts/acid.md)
- [Закон Деметры](concepts/lod.md)
<!--
https://habr.com/ru/articles/811875/
https://habr.com/ru/articles/811305/
-->
- Закон Деметры <!-- https://backendinterview.ru/architecture/principles.html#%D0%97%D0%B0%D0%BA%D0%BE%D0%BD-%D0%94%D0%B5%D0%BC%D0%B5%D1%82%D1%80%D1%8B -->
- Иммутабельность <!-- https://backendinterview.ru/architecture/principles.html#%D0%98%D0%BC%D0%BC%D1%83%D1%82%D0%B0%D0%B1%D0%B5%D0%BB%D1%8C%D0%BD%D0%BE%D1%81%D1%82%D1%8C -->
- наследование и композиция <!-- https://backendinterview.ru/architecture/principles.html#%D0%9F%D1%80%D0%B5%D0%B4%D0%BF%D0%BE%D1%87%D0%B8%D1%82%D0%B0%D0%B9%D1%82%D0%B5-%D0%BA%D0%BE%D0%BC%D0%BF%D0%BE%D0%B7%D0%B8%D1%86%D0%B8%D1%8E-%D0%BD%D0%B0%D1%81%D0%BB%D0%B5%D0%B4%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8E-%D0%BA%D0%BB%D0%B0%D1%81%D1%81%D0%B0 -->
- Признаки плохого проекта <!-- https://backendinterview.ru/architecture/principles.html#%D0%9F%D1%80%D0%B8%D0%B7%D0%BD%D0%B0%D0%BA%D0%B8-%D0%BF%D0%BB%D0%BE%D1%85%D0%BE%D0%B3%D0%BE-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0 -->

[//]: # (- Ковариантность и контрвариантность)
<!-- https://ru.wikipedia.org/wiki/%D0%9A%D0%BE%D0%B2%D0%B0%D1%80%D0%B8%D0%B0%D0%BD%D1%82%D0%BD%D0%BE%D1%81%D1%82%D1%8C_%D0%B8_%D0%BA%D0%BE%D0%BD%D1%82%D1%80%D0%B0%D0%B2%D0%B0%D1%80%D0%B8%D0%B0%D0%BD%D1%82%D0%BD%D0%BE%D1%81%D1%82%D1%8C_(%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5) -->

[//]: # (https://ru.wikipedia.org/wiki/%D0%A7%D0%B5%D0%BC_%D1%85%D1%83%D0%B6%D0%B5,_%D1%82%D0%B5%D0%BC_%D0%BB%D1%83%D1%87%D1%88%D0%B5)

## Паттерны/шаблоны
### Архитектурные паттерны
<!--
https://citforum.ru/SE/project/pattern/
https://habr.com/ru/companies/alconost/articles/522662/
https://habr.com/ru/articles/871500/
https://systems.education/wis_ddd_architectural_patterns
https://tproger.ru/translations/top-5-arhitekturnyh-patternov-dlja-raspredeljonnyh-sistem
https://blog.skillfactory.ru/glossary/pattern/
https://vk.com/@testers-ot-mvc-do-eda
https://proglib.io/p/7-arhitekturnyh-patternov-kotorye-dolzhen-znat-kazhdyy-programmist-2023-05-22
https://tproger.ru/translations/top-5-arhitekturnyh-patternov-dlja-raspredeljonnyh-sistem
https://tproger.ru/articles/topovye-patterny-dlya-razrabotki-arhitektury-po
https://tproger.ru/articles/monolit-ili-mikroservisy--kak-vybrat-arhitekturu-dlya-novogo-proekta
https://habr.com/ru/companies/serverspace/articles/692916/
https://academy.mediasoft.team/article/patterny-proektirovaniya-dlya-chego-nuzhny-kakimi-byvayut-i-chem-otlichayutsya-ot-arkhitekturnykh/
https://systems.education/software_styles_and_patterns_with_cheatsheet
https://habr.com/ru/articles/856452/
https://bigdataschool.ru/blog/architecture-patterns-for-distributed-systems.html
https://proglib.io/p/9-osnovnyh-patternov-dlya-proektirovaniya-raspredelennyh-sistem-2024-07-30
https://medium.com/nuances-of-programming/5-%D0%B2%D0%B5%D0%B4%D1%83%D1%89%D0%B8%D1%85-%D1%88%D0%B0%D0%B1%D0%BB%D0%BE%D0%BD%D0%BE%D0%B2-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F-%D1%80%D0%B0%D1%81%D0%BF%D1%80%D0%B5%D0%B4%D0%B5%D0%BB%D0%B5%D0%BD%D0%BD%D1%8B%D1%85-%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC-b67e9805fee8
https://habr.com/ru/companies/otus/articles/576766/
https://habr.com/ru/companies/otus/articles/754712/
-->
- Anemic Domain Model (антипаттерн?) <!-- https://emacsway.github.io/ru/anemic-domain-model/ -->
- N-tier: многоуровневая архитектура (N — кол-во слоёв)
- Layered: слоистая архитектура (Onion architecture / Hexagonal Architecture)
- Паттерн многослойной архитектуры
- Clean Architecture: чистая архитектура
- Event-Driven Architecture: событийно-ориентированная архитектура.
- DDD (Data-driven development)
- DDD (Domain-driven development) 
- SOA (Service-Oriented Architecture) Сервис-ориентированная архитектура
- Event Sourcing
- Dataflow: поток данных
- Inversion of Control,
- Dependency Inversion,
- Dependency Injection
- Порты и адаптеры
- Многоуровневая архитектура
- Каналы и фильтры
- Клиент — сервер
- Модель — представление — контроллер
- Управляемая событиями архитектура
- Архитектура на основе микросервисов
- MVC (Model-View-Controller)
- MVVM (Model-View-ViewModel)
- HMVC (Hierarchical model–view–controller)
- MVP (Model-View-Presenter)
- State-Model-View (SMV)
- Двухфазная фиксация (2PC)
- Saga
- PageController
- FrontController
- ActiveRecord
- Data Mapper
- Делегирование (Delegation)
- Lazy Load (Ленивая Загрузка)
- Registry (реестр)
- Паттерн автоматического выключения (Circuit Breaker)
- Паттерн источника событий (Event sourcing)
- Паттерн SideCar
- Паттерн CQRS (Command and Query Responsibility Segregation)
- Паттерн Rate Limiting
- Strangler Fig
- Паттерн Health Endpoint Monitoring
- Реплицированные сервисы с распределением нагрузки (RLBS)
- Load Balancer
- Retry (exponential backoff with jitter)
- Database per service
- Шардинг
- Упреждающая журнализация (Write-Ahead Log)
- Split-Brain паттерн
- Направленная отправка (Hinted Handoff)
- Чтение с восстановлением (Read Repair)
- Distributed Monolith (антипаттерн)
- Микролиты (антипаттерн)
- Многослойность (антипаттерн)
- Монолит
- Микросервисы (MSA, Microservice architecture)
Распиливание монолита <!-- 
https://cloud.vk.com/blog/26-osnovnyh-patternov-mikroservisnoj-razrabotki/
https://habr.com/ru/companies/reksoft/articles/864206/
-->
- Decomposition by Domain (Разделение по доменам)
- Decomposition by Business Capability (Разделение по бизнес-возможностям)
- Decomposition by Data (Разделение по данным)
- Decomposition by UI (Разделение по пользовательскому интерфейсу)
- Decomposition by Deployment (Разделение по развертыванию)
- Decomposition by Communication Protocol (Разделение по протоколу коммуникации)
- Domain-driven design
- [WIP: Архитектурные шаблоны (паттерны)](patterns/architectural/architectural-patterns.md)
- [WIP: Предметно-ориентированное проектирование (DDD, Domain-Driven Design)](patterns/architectural/domain-driven-design.md)

### Паттерны микросервисов
<!--
https://habr.com/ru/companies/slurm/articles/679906/
https://habr.com/ru/companies/slurm/articles/681326/
https://proglib.io/p/18-osnovnyh-patternov-mikroservisnoy-arhitektury-2024-07-23
https://cloud.vk.com/blog/26-osnovnyh-patternov-mikroservisnoj-razrabotki/
https://systems.education/microservices-architecture-pattern
https://habr.com/ru/companies/reksoft/articles/864206/
https://habr.com/ru/companies/reksoft/articles/875270/
https://habr.com/ru/companies/piter/articles/275633/
https://dzen.ru/a/ZEoLx3ca-AKQ3cQ7
-->
- [WIP: Паттерн Saga](patterns/microservices/saga.md)
- Stateless Services (Сервисы без состояния)
- Async Messaging (Асинхронный обмен сообщениями)
- Database per Service (База данных для каждого сервиса)
- Smart Endpoints, Dumb Pipes (Умные конечные точки, глупые каналы)
- Consumer-Driven Contracts (Контракты, определяемые потребителем)
- Shadow Deployment (Теневое развертывание)
- Backends for Frontends (BFF, Бэкенды для фронтендов)
- Sidecar (Вспомогательный сервис)
- Retry (Повторная попытка)
- Polyglot Persistence (Многовариантное хранение)
- Data Sharding (Шардинг данных)
- Command Query Responsibility Segregation (CQRS, Разделение команд и запросов)
- Event Sourcing (Источник событий)
- Saga Pattern (Сага)
- Bulkhead (Отсек, Переборка)
- Circuit Breaker (Предохранитель)
- API Gateway (API-шлюз)
- Service Registry (Реестр сервисов)
???
- Шаблон «API-композиция» (API Composition)
- Шаблон «Поиск событий» (Event Sourcing)
- Шаблон «Сборка пользовательского интерфейса на стороне клиента» (Client-Side UI Composition)
- Шаблон «Сборка фрагментов страниц на стороне сервера» (Server-Side Page Fragment Composition)
- Шаблон «Обнаружение сервисов на стороне клиента» (Client-Side Service Discovery)
- Шаблон «Обнаружение сервисов на стороне сервера» (Server-Side Service Discovery)
- Шаблон «Экземпляр сервиса на хост» (Service Instance Per Host)
- Шаблон «Сине-зеленое развертывание» (Blue-Green Deployment)
- Шаблон «Агрегация логов» (Log Aggregation)
- Шаблон «Распределенная трассировка» (Distributed Tracing)
- Шаблон «Проверки здоровья» (Health Check)
- Шаблон «Посредник» («Посол», Ambassador)
- Шаблон «Тестирование контрактов, ориентированных на потребителя» (Consumer-Driven Contract Testing)
- Шаблон «Внешняя конфигурация» (External Configuration)

### Паттерны проектирования
<!--
https://habr.com/ru/articles/804339/
https://habr.com/ru/articles/716412/
https://backendinterview.ru/architecture/gof.html
https://citforum.ru/SE/project/pattern/
https://doka.guide/tools/architecture-and-design-patterns/
Gangs of Four (GoF) Design Patterns
-->

#### Паттерны GoF
- [WIP: GoF: Поведенческий: Цепочка обязанностей (Chain of Responsibility)](patterns/design/gof.behavioral.chain-of-responsibility.md)
- [WIP: GoF: Поведенческий: Команда (Command)](patterns/design/gof.behavioral.command.md)
- [WIP: GoF: Поведенческий: Итератор (iterator)](patterns/design/gof.behavioral.iterator.md)
- [WIP: GoF: Поведенческий: Посредник (Mediator)](patterns/design/gof.behavioral.mediator.md)
- [WIP: GoF: Поведенческий: Снимок (Memento)](patterns/design/gof.behavioral.memento.md)
- [WIP: GoF: Поведенческий: Наблюдатель (Observer)](patterns/design/gof.behavioral.observer.md)
- [WIP: GoF: Поведенческий: Состояние (State)](patterns/design/gof.behavioral.state.md)
- [WIP: GoF: Поведенческий: Стратегия (Strategy)](patterns/design/gof.behavioral.strategy.md)
- [WIP: GoF: Поведенческий: Шаблонный метод (Template Method)](patterns/design/gof.behavioral.template-method.md)
- [WIP: GoF: Поведенческий: Посетитель (Visitor)](patterns/design/gof.behavioral.visitor.md)
- [WIP: GoF: Порождающий: Абстрактная Фабрика (Abstract Factory)](patterns/design/gof.generative.abstract-factory.md)
- [WIP: GoF: Порождающий: Строитель (Builder)](patterns/design/gof.generative.builder.md)
- [WIP: GoF: Порождающий: Фабрика (Factory, Factory Method)](patterns/design/gof.generative.factory-method.md)
- [WIP: GoF: Порождающий: Прототип (Prototype)](patterns/design/gof.generative.prototype.md)
- [WIP: GoF: Порождающий: Одиночка (Singleton)](patterns/design/gof.generative.singleton.md)
- [WIP: GoF: Структурный: Адаптер (Adapter)](patterns/design/gof.structural.adapter.md)
- [WIP: GoF: Структурный: Мост (Bridge)](patterns/design/gof.structural.bridge.md)
- [WIP: GoF: Структурный: Компоновщик (Composite)](patterns/design/gof.structural.composite.md)
- [WIP: GoF: Структурный: Декоратор (Decorator)](patterns/design/gof.structural.decorator.md)
- [WIP: GoF: Структурный: Фасад (Facade)](patterns/design/gof.structural.facade.md)
- [WIP: GoF: Структурный: Легковес (Flyweight)](patterns/design/gof.structural.flyweight.md)
- [WIP: GoF: Структурный: Заместитель (Proxy)](patterns/design/gof.structural.proxy.md)

#### Паттерны GRASP
- [WIP: GRASP: Контроллер (Controller)](patterns/design/grasp.controller.md)
- [WIP: GRASP: Создатель (Creator)](patterns/design/grasp.creator.md)
- [WIP: GRASP: Высокое зацепление (High Cohesion)](patterns/design/grasp.high-cohesion.md)
- [WIP: GRASP: Перенаправление (Indirection)](patterns/design/grasp.indirection.md)
- [WIP: GRASP: Информационный эксперт (Information Expert)](patterns/design/grasp.information-expert.md)
- [WIP: GRASP: Низкая связанность (Low Coupling)](patterns/design/grasp.low-coupling.md)
- [WIP: GRASP: Полиморфизм (Polymorphism)](patterns/design/grasp.polymorphism.md)
- [WIP: GRASP: Устойчивый к изменениям (Protected Variations)](patterns/design/grasp.protected-variations.md)
- [WIP: GRASP: Чистая выдумка (Pure Fabrication)](patterns/design/grasp.pure-fabrication.md)

[//]: # (- Репозиторий &#40;Repository&#41;)
<!--
https://habr.com/ru/articles/248505/
https://gist.github.com/maestrow/594fd9aee859c809b043
https://habr.com/ru/articles/316836/
https://docs.nestjs.com/
-->

## Структуры данных

- [Структуры данных](data-structures/data-structures.md)

## Алгоритмы
- [WIP: Big O. Оценка сложности алгоритмов](algorithms/big-o.md)

[//]: # (- Алгоритмы сортировки)
<!-- https://blog.skillfactory.ru/sorting-algorithm/ -->

## Код:
- [Внедрение зависимостей (dependency-injection)](code/dependency-injection.md)

## JavaScript
- [JavaScript: Цикл событий (Event loop) и libuv](javascript/event-loop-and-libuv.md)
- [WIP: JavaScript: Промисы (Promises)](javascript/js-promises.md)

- [//]: # (- NestJs)
<!--
https://habr.com/ru/companies/timeweb/articles/663234
https://habr.com/ru/companies/timeweb/articles/666470/
-->

## SQL, Базы данных
- [WIP: Шардирование баз данных](sql-and-db/db-sharding.md)
- [Транзакции]([sql-and-db](transactions.md)) <!-- https://ru.wikipedia.org/wiki/ACID -->

[//]: # (- Типы баз данных)

### PostgreSQL

[//]: # (- Виды индексов)

[//]: # (- Транзакции <!-- https://postgrespro.ru/docs/postgrespro/10/tutorial-transactions  https://habr.com/ru/articles/843794/  https://postgrespro.ru/docs/postgrespro/9.6/transaction-iso  https://habr.com/ru/articles/860982/  https://postgrespro.ru/docs/postgresql/13/plpgsql-transactions  https://postgrespro.ru/docs/enterprise/9.6/atx -->)

[//]: # (- GROUP BY <!-- https://postgrespro.ru/docs/postgresql/9.6/queries-table-expressions -->)

[//]: # (- HAVING <!-- https://postgrespro.ru/docs/postgresql/9.6/queries-table-expressions -->)

[//]: # (- GROUPING SETS <!-- https://postgrespro.ru/docs/postgresql/9.6/queries-table-expressions -->)

[//]: # (- CUBE <!-- https://postgrespro.ru/docs/postgresql/9.6/queries-table-expressions -->)

[//]: # (- ROLLUP <!-- https://postgrespro.ru/docs/postgresql/9.6/queries-table-expressions -->)

[//]: # (- Оконные функции)

[//]: # (- Соединения с сопоставлениями строк &#40;JOIN&#41; <!-- https://blog.skillfactory.ru/glossary/join-sql/  https://ru.hexlet.io/courses/complex-sql-queries/lessons/join/theory_unit  https://ru.wikipedia.org/wiki/Join_&#40;SQL&#41;  https://habr.com/ru/articles/655919/  https://postgrespro.ru/docs/postgresql/9.6/queries-table-expressions  https://postgrespro.ru/docs/postgrespro/9.5/tutorial-join -->)

### MongoDB

[//]: # (- Транзакции)

## Флоу в системах контроля версий
<!--
https://habr.com/ru/companies/avito/articles/680522/
+ Git Flow
+ GitLab flow
и т.п.
-->

## Мониторинги
- [WIP: Мониторинг сервисов](services-monitoring.md)

## Управление
- [WIP: Метрики сотрудников](management/employee-metrics.md)

# Вопросы собеседований
<!--
https://habr.com/ru/articles/770522/
-->

## JavaScript
1. [Очистить массив от повторов](tasks/js.clean-doubles-from-array.md)
1. [Проверить, является ли строка зеркальной](tasks/js.is-mirrored-string.md)
1. [Проверить, является ли строка палиндромом](tasks/js.is-palindrome-string)
1. [Перевернуть строку](tasks/js.revert-string.md)

## SQL
1. [Выборка дублирующихся записей](tasks/sql.search-doubles.md)
