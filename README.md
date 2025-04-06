# Programming Cheatsheets (Шпаргалки по программированию) <a name="pagestart"></a>

> [!TIP]
> Если вы что-то не можете объяснить шестилетнему ребёнку, вы сами этого не понимаете (c) Альберт Эйнштейн

Это просто набор кратких описаний, предназначенный, в первую очередь, структурировать знания и быстро вспомнить, то что знаешь, но давно не использовал на практике. Так же будет полезен для подготовки к собеседованиям и просто освежить знания. Если окажется полезным кому-то еще, то буду только рад. :)

В некоторых текстах присутствуют вставки, озаглавленные AIUI (As I Understand It - насколько я понимаю) - это блоки с краткой выжимкой того, как я понимаю описание, тему, понятие.

> [!IMPORTANT]
> Если вы заметили ошибку, неточность, нехватку информации, пожалуйста, сообщите мне.

<!--
https://backendinterview.ru/index.html - аналог моей доки
https://bool.dev/blog/detail/voprosy-na-sobesedovanii-dlya-senior-net-developer - много полезной инфы безотносительно языка
Uniform interface - почитать и добавить
Persistence Context - почитать и добавить
JWT token - описать
-->

---
## Парадигмы <a name="paradigms"></a>

> [!TIP]
> Компьютер хорошо выполняет инструкции, а не читает ваши мысли.

<!--
https://ru.wikipedia.org/wiki/%D0%9F%D0%B0%D1%80%D0%B0%D0%B4%D0%B8%D0%B3%D0%BC%D0%B0_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F
-->
### Основные модели <a name="paradigms-models"></a>
- WIP: [Декларативное программирование](paradigms/models/declarative.md)
- WIP: [Императивное программирование](paradigms/models/imperative.md)
- WIP: [Логическое программирование](paradigms/models/logical.md)
- WIP: [Объектно-ориентированное программирование (ООП)](paradigms/models/object-oriented.md)
  - WIP: [Компонентно-ориентированное программирование](paradigms/models/component-oriented.md)
  - WIP: [Прототипно-ориентированное программирование](paradigms/models/prototype-oriented.md)
  - WIP: [Агентно-ориентированное программирование](paradigms/models/agent-oriented.md)
- WIP: [Структурное программирование](paradigms/models/structural.md)
- WIP: [Функциональное программирование](paradigms/models/functional.md)
- WIP: [Экстремальное программирование](paradigms/models/extreme.md)

### Подходы и приёмы <a name="paradigms-techniques"></a>
- WIP: [Автоматное программирование](paradigms/techniques/automatic.md)
- WIP: [Аппликативное программирование](paradigms/techniques/applicative.md)
- WIP: [Аспектно-ориентированное программирование (АОП)](paradigms/techniques/aspect-oriented.md)
- WIP: [Грамотное программирование](paradigms/techniques/literate.md)
- WIP: [Доказательное программирование](paradigms/techniques/evidential.md)
- WIP: [Контрактное программирование](paradigms/techniques/contractual.md)
- WIP: [Обобщённое программирование](paradigms/techniques/generalized.md)
- WIP: [Порождающее программирование](paradigms/techniques/generative.md)
- WIP: [Процедурное программирование](paradigms/techniques/procedural.md)
- WIP: [Событийно-ориентированное программирование](paradigms/techniques/event-oriented.md)

---
## Концепции, понятия, термины <a name="concepts"></a>

> [!TIP]
> Пишите код так, как будто поддерживать его будет склонный к насилию психопат, который знает, где вы живёте (c) Джон Ф. Вудс

<!--
https://medium.com/nuances-of-programming/10-%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%81%D1%82%D1%81%D0%BA%D0%B8%D1%85-%D1%82%D0%B5%D1%80%D0%BC%D0%B8%D0%BD%D0%BE%D0%B2-%D0%BD%D0%B0-%D0%BF%D0%BE%D0%BD%D1%8F%D1%82%D0%BD%D0%BE%D0%BC-%D1%8F%D0%B7%D1%8B%D0%BA%D0%B5-8c2cb31fcda4
-->

- WIP: [Признаки плохого проекта](concepts/bad-project.md)

### Правила <a name="concepts-rules"></a>
- **[Требования ACID](concepts/rules/acid.md)** - Набор требований к транзакционной системе для надёжности и предсказуемости.
  - [Атомарность](concepts/rules/acid.md#atomicity) - Никакая транзакция не должна быть зафиксирована в системе частично.
  - [Изоляция](concepts/rules/acid.md#isolation) - Во время выполнения транзакции параллельные транзакции не должны оказывать влияния на её результат.
  - [Согласованность](concepts/rules/acid.md#consistency) - Завершенная транзакция сохраняет согласованность базы данных.
  - [Устойчивость](concepts/rules/acid.md#durability) - Независимо от проблем, изменения, сделанные успешно завершённой транзакцией, должны остаться сохранёнными.
- **[Принцип DRY](concepts/rules/dry.md)** - Не повторяй свой код. Избегайте дублирования кода без острой необходимости.
- **[Принципы KISS](concepts/rules/kiss.md)** - Делай это проще. Разбивайте задачи, сначала решение задачи, потом код. Делайте классы и методы маленькими. Не бойтесь избавляться от кода.
- **[Принципы SOLID](concepts/rules/solid.md)** - Способствует созданию такой системы, которую будет легко поддерживать и расширять в течение долгого времени.
  - [S](concepts/rules/solid.md#s) - Принцип единственной ответственности. Предлагает разделять универсальные классы на конкретные, что сделает их простыми и лёгкими в обслуживании.
  - [O](concepts/rules/solid.md#o) - Принцип открытости/закрытости. Сущности должны быть открыты для расширения, но закрыты для модификации.
  - [L](concepts/rules/solid.md#l) - Принцип подстановки Лисков. Производный класс должен сохранять все свойства базового класса и не изменять их семантику.
  - [I](concepts/rules/solid.md#i) - Принцип разделения интерфейса. Слишком большие интерфейсы необходимо разделять на более маленькие и специфические.
  - [D](concepts/rules/solid.md#d) - Принцип инверсии зависимостей. Модули верхнего уровня не должны зависеть от модулей нижнего уровня. Оба типа модулей должны зависеть от абстракций.
- **[Принципы YAGNI](concepts/rules/yagni.md)** - Не стоит создавать код, который может понадобиться потом, так как "потом" может никогда не наступить.
- **[Закон Деметры](concepts/rules/lod.md)** - Можно вызывать только методы/переменные самого класса или методы и переменные класса переданного как зависимость.
- **[Подход MIT](concepts/rules/mit.md)** - Подход к разработке делающий упор на реализации, логичности и покрытию максимального количества важных ситуаций.
- **[Подход "Чем хуже, тем лучше"](concepts/rules/worse-is-better.md)** - Подход к разработке, объявляющий простоту реализации и интерфейса более важными, чем другие свойства системы.

### Отношения <a name="concepts-relations"></a>
- **[Агрегирование (Aggregation)](concepts/relations/aggregation.md)** - Отношения между объектами, когда при создании нового объекта ему передаются уже существующие объекты.
- **[Ассоциация (Association)](concepts/relations/association.md)** - Отношения между объектами, когда один объект может вызвать другой объект, чтобы выполнить действия от его имени.
- **[Ковариантность и контрвариантность](concepts/relations/covariance-and-contravariance.md)** - Способы переноса наследования типов на производные от них типы.
  - [Инвариантность (Invariance)](concepts/relations/covariance-and-contravariance.md#invariance) - Наследование типов не переносится на производные.
  - [Ковариантность (Covariance)](concepts/relations/covariance-and-contravariance.md#covariance) - Перенос наследования типов на производные от них типы в прямом порядке.
  - [Контравариантность (Contravariance)](concepts/relations/covariance-and-contravariance.md#contravariance) - Перенос наследования типов на производные от них типы в обратном порядке.
- **[Композиция (Composition)](concepts/relations/composition.md)** - Отношения между объектами, когда при создании нового объекта создаются все необходимые ему дополнительные объекты.
- **[Наследование (Inheritance)](concepts/relations/inheritance.md)** - Когда класс наследуется от родительского класса, он приобретает все характеристики родительского класса.
- **[Отношение HAS-A](concepts/relations/has-a.md)** - Сокращенное описание "класс В содержит параметр с экземпляром(-ами) класса С".
- **[Отношение IS-A](concepts/relations/is-a.md)** - Сокращенное описание "класс С является наследником/расширением/реализацией класса/интерфейса В".

### Функции, методы <a name="concepts-functions"></a>
- **[Анонимная функция (Anonymous function)](concepts/functions/anonymous-function.md)** - Объявляется в месте использования и не получает уникального идентификатора для доступа к ней.
- **[Замыкание (Closure)](concepts/functions/closure.md)** - Функция ссылается на переменные, не содержащиеся в её теле.
- WIP: [Каррирование (Carrining)](concepts/functions/carrining.md)
- **[Лямбда-выражение (Lambda expression)](concepts/functions/lambda-expression.md)** - Специальный синтаксис для объявления анонимных функций.
- **[Мемоизация, Табулирование, Кэш (Memoization)](concepts/functions/memoization.md)** - Сохранение результатов выполнения функций для предотвращения повторных вычислений.
- WIP: [Перегрузка (Overload)](concepts/functions/overload.md)
- **[Рекурсия (Recursion)](concepts/functions/recursion.md)** - Поведение функции, при котором она вызывает сама себя.
- **[Функции первого (высшего) класса (порядка)](concepts/functions/first-order-functions.md)** - Принимает в качестве аргументов другие функции и/или возвращающая другую функцию.
- **[Чистая функция (Pure function)](concepts/functions/pure-function.md)** - Зависит только от своих объявленных входных данных и своей реализации для получения результата.

### Свойства <a name="concepts-properties"></a>
- **[Абстракция (Abstraction)](concepts/properties/abstraction.md)** - Выделение общих характеристик объектов, их свойств и методов, без деталей реализации.
- **[Идемпотентность (Idempotency)](concepts/properties/idempotency.md)** - Когда повторное применение операции или обращение к объекту будет давать тот же результат, что и при первом.
- **[Иммутабельность (Immutability)](concepts/properties/immutability.md)** - После создания данные или структура, которая их содержит, не могут быть изменены.
- **[Инкапсуляция (Encapsulation)](concepts/properties/encapsulation.md)** - Ограждает группу методов или данных от внешнего вмешательства или неправильного использования.
- WIP: [Полиморфизм (Polymorphism)](concepts/properties/polymorphism.md)
- **[Реентерабельность (Reentrant)](concepts/properties/reentrant.md)** - Oдна и та же инструкция программы может быть совместно использована несколькими пользователями или процессами.

### Прочее <a name="concepts-others"></a>
- WIP: [Без сохранения состояния (Stateless)](concepts/others/stateless.md)
- WIP: [Детерминирование (Determination)](concepts/others/determination.md)
- WIP: [Зацепление (Coupling)](concepts/others/coupling.md)
- WIP: [Класс (Class)](concepts/others/class.md)
- WIP: [Конечный автомат (Finite-state machine, FSM)](concepts/others/finite-state-machine.md)
- WIP: [Прототип (Prototype)](concepts/others/prototype.md)
- WIP: [Связность|связанность (Cohesion)](concepts/others/cohesion.md)
- WIP: [Сохранение состояния (Statefull)](concepts/others/statefull.md)
- WIP: [Устойчивость (Persistence)](concepts/others/persistence.md)

---
## Структуры и типы данных <a name="data-structures"></a>

> [!TIP]
> Вот вы говорите "электронный документооборот". А вы знаете сколько из-за него ежегодно вырубают бинарных деревьев?

- WIP: [Структуры данных](data-structures/data-structures.md)
- WIP: [Абстрактные типы данных](data-structures/abstract-data-types.md)
- **[Простые структуры данных - типы данных](data-structures/simple-data-structures.md)** - Примитивы, базовые элементы. Составная часть сложных структур данных.
- **[Сложные (интегрированные) структуры данных:](data-structures/complex-data-structures.md)** - Состоят из примитивов или других структур данных.
  - [Статические](data-structures/static.md) - Структурированное множество простых структур.
  - [Полустатические](data-structures/semi-static.md) - Последовательность данных, связанная отношениями линейного списка.
  - [Динамические](data-structures/dynamic.md) - Не обладают постоянным размером. Обеспечивает высокую изменчивость структуры.
  - [Линейные](data-structures/linear.md)
  - [Нелинейные](data-structures/nonlinear.md)
  - [Связные и несвязные](data-structures/coherent-and-incoherent.md)

<!--
https://ru.wikipedia.org/wiki/%D0%A1%D0%B2%D1%8F%D0%B7%D0%BD%D1%8B%D0%B9_%D1%81%D0%BF%D0%B8%D1%81%D0%BE%D0%BA
https://www.bigocheatsheet.com/
http://aisd-kubsau0.1gb.ru/lections/lect-kurs-isit/lect2_isit.html
Деки - что за тип?
-->
### Описание структур данных <a name="data-structures-descriptions"></a>
- **[Массив (Array), Вектор (Vector), Матрица (Matrix)](data-structures/descriptions/arrays.md)**
  - [Динамический массив (Dynamic arrays)](data-structures/descriptions/arrays.dynamic.md)
  - [Ассоциативные массивы (Associative Arrays)](data-structures/descriptions/arrays.associative.md)
- **[Стеки (Stacks)](data-structures/descriptions/stacks.md)**
- **[Очереди (Queues)](data-structures/descriptions/queues.md)**
- **[Списки (Lists)](data-structures/descriptions/lists.md)**
  - WIP: [Односвязнный (однонаправленный) список (Single-linked list)](data-structures/descriptions/lists.single-linked.md)
  - WIP: [Двусвязнный (двунаправленный) список (Double-linked list)](data-structures/descriptions/lists.double-linked.md)
  - WIP: [Кольцевой связный список (Ring linked list)](data-structures/descriptions/lists.ring-linked.md)
  - WIP: [Развёрнутый связный список (Expanded linked list)](data-structures/descriptions/lists.expanded-linked.md)
  - WIP: [Список с пропусками (Skip List)](data-structures/descriptions/lists.skip.md)
  - WIP: [XOR-связный список (XOR linked list)](data-structures/descriptions/lists.xor-linked.md)
- **[Хэш-таблицы, Хэш-мапы (Hash tables, Hash Maps)](data-structures/descriptions/hash-maps.md)**
- **[Множества, Хэш-сеты (Sets, Hash Sets)](data-structures/descriptions/hash-sets.md)**
- **[Карты, Словари (Maps, Dictionaries)](data-structures/descriptions/maps.md)**
- **[Графы (Graphs)](data-structures/descriptions/graphs.md)**
- WIP: [Деревья (Trees)](data-structures/descriptions/trees.md)
  - WIP: [Бинарное дерево (Binary tree)](data-structures/descriptions/trees.binary.md)
  - WIP: [Бинарное дерево поиска (Binary search tree)](data-structures/descriptions/trees.binary-search.md)
  - WIP: [Красно-чёрное дерево (Red-black tree)](data-structures/descriptions/trees.red-black.md)
  - WIP: [AVL-дерево (AVL tree)](data-structures/descriptions/trees.avl.md)
  - WIP: [T-дерево (T-tree)](data-structures/descriptions/trees.t.md)
  - WIP: [Декартово дерево (Cartesian tree)](data-structures/descriptions/trees.cartesian.md)
  - WIP: [B-дерево (B-tree)](data-structures/descriptions/trees.b.md)
  - WIP: [R-дерево (B-tree)](data-structures/descriptions/trees.r.md)
  - WIP: [Splay дерево (Splay tree)](data-structures/descriptions/trees.splay.md)
  - WIP: [KD дерево (KD tree)](data-structures/descriptions/trees.kd.md)
  - WIP: [Деревья квадрантов (Quadrant trees)](data-structures/descriptions/trees.quadrant.md)
  - WIP: [K-мерные деревья (K-dimensional trees)](data-structures/descriptions/trees.k-dimensional.md)
  - WIP: [Префиксные деревья, Бор, Нагруженные деревья (Trie, Prefix Trees)](data-structures/descriptions/trees.trie.md)
- **[Кучи (Heaps)](data-structures/descriptions/heaps.md)**
- **[Запись (Record)](data-structures/descriptions/records.md)**
- **[Кортеж (Tuple)](data-structures/descriptions/tuple.md)**

---
## Алгоритмы <a name="algorithms"></a>

> [!TIP]
> Вы никогда не задумывались, какое количество психических сил потрачено разработчиками на попытки понять различие между алгоритмом и программой...

<!--
http://aisd-kubsau0.1gb.ru/lections/lect-kurs-isit/lect2_isit.html
https://sky.pro/wiki/python/osnovnye-algoritmy-v-programmirovanii/
https://skillbox.ru/media/code/chto-takoe-algoritmy-i-kakimi-oni-byvayut/
https://dtf.ru/u/868521-hypeway-studio/2081676-chto-takoe-algoritmy-programmirovaniya-osnovy-i-primenenie
https://blog.skillfactory.ru/sorting-algorithm/
https://habr.com/ru/companies/sberbank/articles/756894/
https://proglib.io/p/12-algoritmov-kotorye-dolzhen-znat-kazhdyy-razrabotchik-obyasnyaem-na-gifkah-2022-11-21
https://itproger.com/news/chto-takoe-algoritmi-programmirovaniya-osnovi-i-primenenie
https://sky.pro/wiki/javascript/osnovnye-algoritmy-programmirovaniya-chto-nuzhno-znat-kazhdomu-programmistu/
https://habr.com/ru/companies/piter/articles/719228/
https://decode.kz/blog/category/top-8-algorithms-every-programmer-should-know
https://tproger.ru/experts/7
https://tproger.ru/articles/algoritm-dejkstry--kak-rabotaet-i-gde-ispolzuetsya
https://purpleschool.ru/blog/algoritmy-osnovy-programmirovaniya-dlya-nachinayushchih
https://proglib.io/p/required-programmer-algorithms
https://education.yandex.ru/handbook/algorithms
https://blog.skillfactory.ru/glossary/algoritm/
-->
- WIP: [Big O. Оценка сложности алгоритмов](algorithms/big-o.md)

### Алгоритмы сортировки <a name="algorithms-sort"></a>
- WIP: [Быстрая сортировка](algorithms/sort/quick.md)
- WIP: [Параллельная кеш-независимая сортировка](algorithms/sort/parallel-cache-independent.md)
- WIP: [Пузырьковая сортировка](algorithms/sort/bubble.md)
- WIP: [Рандомизированный алгоритм](algorithms/sort/randomized.md)
- WIP: [Сортировка вставками](algorithms/sort/insertion.md)
- WIP: [Сортировка выбором](algorithms/sort/selection.md)
- WIP: [Сортировка кучей](algorithms/sort/heap.md)
- WIP: [Сортировка слиянием](algorithms/sort/merge.md)

### Поисковые алгоритмы <a name="algorithms-search"></a>
- WIP: [Бинарный поиск](algorithms/search/binary.md)
- WIP: [Линейный поиск](algorithms/search/linear.md)
- WIP: [Поиск в массиве](algorithms/search/in-array.md)

### Алгоритмы работы с данными <a name="algorithms-data"></a>
- WIP: [Обход связного списка](algorithms/data/linked-list-traversal.md)
- WIP: [Операции с очередью](algorithms/data/queue-operations.md)
- WIP: [Операции со стэком](algorithms/data/stack-operations.md)
- WIP: [Работа с хеш-таблицами](algorithms/data/hash-table-operations.md)
- WIP: [Разворачивание однонаправленного списка](algorithms/data/single-linked-list-reversal.md)

### Графы и деревья <a name="algorithms-graph-or-tree"></a>
- WIP: [Алгоритм Дейкстры](algorithms/graph-or-tree/dijkstra-algorithm.md)
- WIP: [Алгоритм Флойда-Уоршелла](algorithms/graph-or-tree/floyd-warshall-algorithm.md)
- WIP: [Алгоритмы работы с бинарными деревьями](algorithms/graph-or-tree/binary-tree-algorithms.md)
- WIP: [Градиентный спуск](algorithms/graph-or-tree/gradient-descent.md)
- WIP: [Поиск (обход) в глубину](algorithms/graph-or-tree/depth-first-search.md)
- WIP: [Поиск (обход) в ширину](algorithms/graph-or-tree/breadth-first-search.md)

### Рекурсия (рекурсивные алгоритмы) <a name="algorithms-recursion"></a>
- WIP: [Факториал](algorithms/recursion/factorial.md)
- WIP: [Фибоначчи](algorithms/recursion/fibonacci.md)

### Динамическое программирование <a name="algorithms-dynamic"></a>
- WIP: [Задача о наибольшей общей подпоследовательности (Longest Common Subsequence)](algorithms/dynamic/largest-common-subsequence-problem.md)
- WIP: [Задача о рюкзаке](algorithms/dynamic/backpack-problem.md)
- WIP: [Расстановка ферзей (Проблема N-ферзей)](algorithms/dynamic/queen-ordering.md)

### Жадные алгоритмы (Greedy Algorithms) || Сжатие данных <a name="algorithms-greedy"></a>
- WIP: [Арифметическое кодирование](algorithms/greedy/arithmetic-coding.md)
- WIP: [Кодирование Хаффмена](algorithms/greedy/huffman-coding.md)
- WIP: [Сжатие подпоследовательностей](algorithms/greedy/subsequence-compression.md)

### Прочее <a name="algorithms-others"></a>
- WIP: [Обмен ключами Диффи-Хеллмана](algorithms/others/key-exchange-diffie-hellman.md)
- WIP: [Символические вычисления](algorithms/others/symbolic-computation.md)

---
## Архитектура, паттерны, модели <a name="patterns"></a>

> [!TIP]
> Всегда мало времени, чтобы разработать проект, но его всегда хватает, чтобы сделать в 2 раза больше багов.

<!--
https://sky.pro/wiki/javascript/arhitekturnye-shablony-v-razrabotke-po/
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
https://design-pattern.ru/patterns/
https://habr.com/ru/articles/334126/
https://tproger.ru/articles/domain-driven-design-davajte-ne-budem-uslozhnyat
https://habr.com/ru/companies/sberbank/articles/781612/
https://tproger.ru/translations/top-5-arhitekturnyh-patternov-dlja-raspredeljonnyh-sistem
https://systems.education/wis_ddd_architectural_patterns
https://habr.com/ru/companies/alconost/articles/522662/
https://habr.com/ru/articles/261171/
12factor.net
Zero Trust архитектуру
-->

### Виды архитектур <a name="patterns-architectures"></a>
- WIP: [Гексагональная архитектура (Hexagonal Architecture)](patterns/architectures/hexagonal.md)
- WIP: [Клиент-серверная архитектура (Client–Server Architecture)](patterns/architectures/client–server.md)
- WIP: [Микролитная архитектура (Microlite architecture)](patterns/architectures/microlite.md)
- WIP: [Микросервисная архитектура (Microservice architecture, MSA)](patterns/architectures/microservice.md)
- WIP: [Микроядерная архитектура (Microkernel architecture)](patterns/architectures/microkernel.md)
- WIP: [Многоуровневая архитектура (N-tier)](patterns/architectures/n-tier.md)
- WIP: [Монолитная архитектура (Monolith architecture)](patterns/architectures/monolith.md)
- WIP: [Одноранговая архитектура (Peer-to-Peer Architecture)](patterns/architectures/peer-to-peer.md)
- WIP: [Поток данных (Dataflow)](patterns/architectures/dataflow.md)
- WIP: [Распределенный монолит (Distributed Monolith)](patterns/architectures/distributed-monolith.md)
- WIP: [Реплицированные сервисы с распределением нагрузки (RLBS)](patterns/architectures/rlbs.md)
- WIP: [Сервис-ориентированная архитектура (Service-Oriented Architecture, SOA)](patterns/architectures/service-oriented.md)
- WIP: [Слоистая архитектура (Onion architecture)](patterns/architectures/onion.md)
- WIP: [Событийно-ориентированная архитектура (Event-Driven Architecture)](patterns/architectures/event-driven.md)
- WIP: [Чистая архитектура (Clean Architecture)](patterns/architectures/clean.md)

### Концепции проектирования <a name="patterns-concepts"></a>
- WIP: [Анемичная модель (Anemic Domain Model)](patterns/concepts/anemic-domain-model.md)
- WIP: [Богатая модель (Rich Domain Model)](patterns/concepts/rich-domain-model.md)
- WIP: [Вертикальное масштабирование (Vertical Scaling)](patterns/concepts/vertical-scaling.md)
- WIP: [Горизонтальное масштабирование (Horizontal Scaling)](patterns/concepts/horizontal-scaling.md)
- WIP: [Ориентированное на данные (Data-Driven Design)](patterns/concepts/data-driven-design.md)
- WIP: [Предметно-ориентированное (Domain-Driven Design, DDD)](patterns/concepts/domain-driven-design.md)
- WIP: [Хостинг статического контента (Static Content Hosting)](patterns/concepts/static-content-hosting.md)
- WIP: [Шардирование (Sharding)](patterns/concepts/sharding.md)

### Архитектурные паттерны <a name="patterns-architectural"></a>
<!--
https://tproger.ru/translations/top-5-arhitekturnyh-patternov-dlja-raspredeljonnyh-sistem
https://systems.education/wis_ddd_architectural_patterns
https://habr.com/ru/companies/alconost/articles/522662/
-->
- **[Внедрение зависимостей (Dependency Injection, DI)](patterns/architectural/di.md)**
- WIP: [Делегирование (Delegation)](patterns/architectural/delegation.md)
- WIP: [Душитель (Strangler Fig)](patterns/architectural/strangler-fig.md)
- WIP: [Иерархические Модель-Представление-Контроллер (Hierarchical model–view–controller, HMVC)](patterns/architectural/hmvc.md)
- WIP: [Инверсия зависимостей (Dependency Inversion Principle, DIP)](patterns/architectural/dip.md)
- WIP: [Инверсия управления (Inversion of Control, IoC)](patterns/architectural/ioc.md)
- WIP: [Каналы и фильтры (Pipes & Filters)](patterns/architectural/pipes-and-filters.md)
- WIP: [Контейнер внедрения зависимостей (Dependency Injection Container, DIC)](patterns/architectural/dic.md)
- WIP: [Контроллер страницы (Page Controller)](patterns/architectural/page-controller.md)
- WIP: [Модель-Представление-Контроллер (Model-View-Controller, MVC)](patterns/architectural/mvc.md)
- WIP: [Модель-Представление-МодельПредставления (Model-View-ViewModel, MVVM)](patterns/architectural/mvvm.md)
- WIP: [Модель-Представление-Представитель (Model-View-Presenter, MVP)](patterns/architectural/mvp.md)
- WIP: [Направленная отправка (Hinted Handoff)](patterns/architectural/hinted-handoff.md)
- WIP: [Обратное проксирование (Reverse Proxy)](patterns/architectural/reverse-proxy.md)
- WIP: [Ограничение скорости (Rate Limiting)](patterns/architectural/rate-limiting.md)
- WIP: [Разделение команд и запросов (Command and Query Responsibility Segregation, CQRS)](patterns/architectural/cqrs.md)
- WIP: [Разделенный мозг (Split-Brain)](patterns/architectural/split-brain.md)
- WIP: [Распределение нагрузки (Load Balancer)](patterns/architectural/load-balancer.md)
- WIP: [Реестр (Registry)](patterns/architectural/registry.md)
- WIP: [Состояние-Модель-Представление (State-Model-View, SMV)](patterns/architectural/smv.md)

#### Преобразование монолита <a name="patterns-monolith"></a>
<!-- 
https://cloud.vk.com/blog/26-osnovnyh-patternov-mikroservisnoj-razrabotki/
https://habr.com/ru/companies/reksoft/articles/864206/
-->
- WIP: [Разделение по бизнес-возможностям (Decomposition by Business Capability)](patterns/monolith/business-capability.md)
- WIP: [Разделение по данным (Decomposition by Data)](patterns/monolith/data.md)
- WIP: [Разделение по пользовательскому интерфейсу (Decomposition by UI)](patterns/monolith/ui.md)
- WIP: [Разделение по предметным областям (Decomposition by Domain)](patterns/monolith/domain.md)
- WIP: [Разделение по протоколу коммуникации (Decomposition by Communication Protocol)](patterns/monolith/communication-protocol.md)
- WIP: [Разделение по развертыванию (Decomposition by Deployment)](patterns/monolith/deployment.md)

#### Паттерны микросервисов <a name="patterns-microservices"></a>
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
https://dzen.ru/a/YKJ99EP6Y0aFqFC1
-->
- WIP: [API-композиция (API Composition)](patterns/microservices/api-composition.md)
- WIP: [API-шлюз (API Gateway)](patterns/microservices/api-gateway.md)
- WIP: [Агрегация логов (Log Aggregation)](patterns/microservices/log-aggregation.md)
- WIP: [Асинхронный обмен сообщениями (Async Messaging)](patterns/microservices/async-messaging.md)
- WIP: [База данных на сервис (Database per service)](patterns/microservices/database-per-service.md)
- WIP: [Бэкенды для фронтендов (Backends for Frontends, BFF)](patterns/microservices/backends-for-frontends.md)
- WIP: [Внешняя конфигурация (External Configuration)](patterns/microservices/external-configuration.md)
- WIP: [Вспомогательный сервис (Sidecar)](patterns/microservices/sidecar.md)
- WIP: [Единая точка входа (Front Controller)](patterns/microservices/front-controller.md)
- WIP: [Источник событий (Event Sourcing)](patterns/microservices/event-sourcing.md)
- WIP: [Контракты, определяемые потребителем (Consumer-Driven Contracts)](patterns/microservices/consumer-driven-contracts.md)
- WIP: [Многовариантное хранение (Polyglot Persistence)](patterns/microservices/polyglot-persistence.md)
- WIP: [Обнаружение сервисов на стороне клиента (Client-Side Service Discovery)](patterns/microservices/client-side-service-discovery.md)
- WIP: [Обнаружение сервисов на стороне сервера (Server-Side Service Discovery)](patterns/microservices/server-side-service-discovery.md)
- WIP: [Отсек, Переборка (Bulkhead)](patterns/microservices/bulkhead.md)
- WIP: [Повторная попытка (Retry)](patterns/microservices/retry.md)
- WIP: [Посол, Посредник (Ambassador)](patterns/microservices/ambassador.md)
- WIP: [Предохранитель, Автовыключение (Circuit Breaker)](patterns/microservices/circuit-breaker.md)
- WIP: [Проверки здоровья (Health Check)](patterns/microservices/health-check.md)
- WIP: [Распределенная трассировка (Distributed Tracing)](patterns/microservices/distributed-tracing.md)
- WIP: [Реестр сервисов (Service Registry)](patterns/microservices/service-registry.md)
- WIP: [Сага (Saga)](patterns/microservices/saga.md)
- WIP: [Сборка пользовательского интерфейса на стороне клиента (Client-Side UI Composition)](patterns/microservices/client-side-ui-composition.md)
- WIP: [Сборка фрагментов страниц на стороне сервера (Server-Side Page Fragment Composition)](patterns/microservices/server-side-page-fragment-composition.md)
- WIP: [Сервисы без состояния (Stateless Services)](patterns/microservices/stateless-services.md)
- WIP: [Сине-зеленое развертывание (Blue-Green Deployment)](patterns/microservices/blue-green-deployment.md)
- WIP: [Теневое развертывание (Shadow Deployment)](patterns/microservices/shadow-deployment.md)
- WIP: [Умные конечные точки, глупые каналы (Smart Endpoints, Dumb Pipes)](patterns/microservices/smart-endpoints-dumb-pipes.md)
- WIP: [Фронтенды для Бэкендов (Frontends for Backends, FFB)](patterns/microservices/frontends-for-backends.md)
- WIP: [Шардинг данных (Data Sharding)](patterns/microservices/data-sharding.md)
- WIP: [Экземпляр сервиса на хост (Service Instance Per Host)](patterns/microservices/service-instance-per-host.md)

### Паттерны работы с БД <a name="patterns-db"></a>
- WIP: [Активная запись (Active Record, AR)](patterns/db/active-record.md)
- WIP: [Двухфазная фиксация (2PC)](patterns/db/2pc.md)
- WIP: [Упреждающая журнализация (Write-Ahead Log)](patterns/db/write-ahead-log.md)
- WIP: [Чтение с восстановлением (Read Repair)](patterns/db/read-repair.md)

### Паттерны проектирования <a name="patterns-design"></a>
<!--
https://ru.wikipedia.org/wiki/%D0%A8%D0%B0%D0%B1%D0%BB%D0%BE%D0%BD_%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F
https://habr.com/ru/articles/136766/
https://habr.com/ru/articles/804339/
https://habr.com/ru/articles/716412/
https://backendinterview.ru/architecture/gof.html
https://citforum.ru/SE/project/pattern/
https://doka.guide/tools/architecture-and-design-patterns/
Gangs of Four (GoF) Design Patterns
-->

#### Паттерны GRASP <a name="patterns-design-grasp"></a>
**G**eneral **R**esponsibility **A**ssignment **S**oftware **P**atterns. Шаблоны проектирования, используемые для решения общих задач по назначению обязанностей классам и объектам. Описано девять GRAPS шаблонов. Паттерны не имеют выраженной структуры, четкой области применения и конкретной решаемой проблемы, а лишь представляют собой обобщенные подходы/рекомендации/принципы, используемые при проектировании дизайна системы. Это распределение ролей и ответственностей между всеми объектами, а также свойства, которыми эти объекты должны обладать для того, чтобы гармонично исполнять свои роли.

- WIP: [GRASP: Высокое зацепление (High Cohesion)](patterns/design/grasp/high-cohesion.md)
- **[GRASP: Информационный эксперт (Information Expert)](patterns/design/grasp/information-expert.md)**
- WIP: [GRASP: Контроллер (Controller)](patterns/design/grasp/controller.md)
- WIP: [GRASP: Низкая связанность (Low Coupling)](patterns/design/grasp/low-coupling.md)
- WIP: [GRASP: Перенаправление (Indirection)](patterns/design/grasp/indirection.md)
- WIP: [GRASP: Полиморфизм (Polymorphism)](patterns/design/grasp/polymorphism.md)
- WIP: [GRASP: Создатель (Creator)](patterns/design/grasp/creator.md)
- WIP: [GRASP: Устойчивый к изменениям (Protected Variations)](patterns/design/grasp/protected-variations.md)
- WIP: [GRASP: Чистая выдумка (Pure Fabrication)](patterns/design/grasp/pure-fabrication.md)

#### Паттерны GoF <a name="patterns-design-gof"></a>
**G**angs **O**f **F**our (Банда четырех). В 1995 году Эрих Гамм, Ричард Хелм, Ральф Джонсон и Джон Влиссидес написали книгу "Design Patterns: Elements of Reusable Object-Oriented Software", в которой применили концепцию типовых паттернов в программировании. В книгу вошли 23 паттерна, решающие различные проблемы объектно-ориентированного дизайна.

- WIP: [GoF: Поведенческий: Итератор (iterator)](patterns/design/gof/behavioral.iterator.md)
- WIP: [GoF: Поведенческий: Команда (Command)](patterns/design/gof/behavioral.command.md)
- WIP: [GoF: Поведенческий: Наблюдатель (Observer)](patterns/design/gof/behavioral.observer.md)
- WIP: [GoF: Поведенческий: Посетитель (Visitor)](patterns/design/gof/behavioral.visitor.md)
- WIP: [GoF: Поведенческий: Посредник (Mediator)](patterns/design/gof/behavioral.mediator.md)
- WIP: [GoF: Поведенческий: Снимок (Memento)](patterns/design/gof/behavioral.memento.md)
- WIP: [GoF: Поведенческий: Состояние (State)](patterns/design/gof/behavioral.state.md)
- WIP: [GoF: Поведенческий: Стратегия (Strategy)](patterns/design/gof/behavioral.strategy.md)
- WIP: [GoF: Поведенческий: Цепочка обязанностей (Chain of Responsibility)](patterns/design/gof/behavioral.chain-of-responsibility.md)
- WIP: [GoF: Поведенческий: Шаблонный метод (Template Method)](patterns/design/gof/behavioral.template-method.md)
- WIP: [GoF: Порождающий: Абстрактная Фабрика (Abstract Factory)](patterns/design/gof/generative.abstract-factory.md)
- WIP: [GoF: Порождающий: Одиночка (Singleton)](patterns/design/gof/generative.singleton.md)
- WIP: [GoF: Порождающий: Прототип (Prototype)](patterns/design/gof/generative.prototype.md)
- WIP: [GoF: Порождающий: Строитель (Builder)](patterns/design/gof/generative.builder.md)
- WIP: [GoF: Порождающий: Фабричный метод (Factory, Factory Method)](patterns/design/gof/generative.factory-method.md)
- WIP: [GoF: Структурный: Адаптер (Adapter)](patterns/design/gof/structural.adapter.md)
- WIP: [GoF: Структурный: Декоратор (Decorator)](patterns/design/gof/structural.decorator.md)
- WIP: [GoF: Структурный: Заместитель (Proxy)](patterns/design/gof/structural.proxy.md)
- WIP: [GoF: Структурный: Компоновщик (Composite)](patterns/design/gof/structural.composite.md)
- WIP: [GoF: Структурный: Легковес (Flyweight)](patterns/design/gof/structural.flyweight.md)
- WIP: [GoF: Структурный: Мост (Bridge)](patterns/design/gof/structural.bridge.md)
- WIP: [GoF: Структурный: Фасад (Facade)](patterns/design/gof/structural.facade.md)

#### Прочие паттерны <a name="patterns-design-others"></a>
<!--
https://design-pattern.ru/patterns/data-mapper.html
https://qna.habr.com/q/390215
https://designpatternsphp.readthedocs.io/ru/latest/Structural/DataMapper/README.html
https://habr.com/ru/articles/248505/
https://gist.github.com/maestrow/594fd9aee859c809b043
https://habr.com/ru/articles/316836/
https://docs.nestjs.com/
-->
- WIP: [Ленивая загрузка (Lazy Load)](patterns/design/others/lazy-load.md)
- WIP: [Поставщик/потребитель (Producer/Consumer)](patterns/design/others/producer-consumer.md)
- WIP: [Преобразователь данных (Data Mapper)](patterns/design/others/data-mapper.md)
- WIP: [Репозиторий (Repository)](patterns/design/others/repository.md)

---
## Протоколы и клиент-серверное взаимодействие <a name="protocols"></a>

> [!TIP]
> А ты не чувствуешь красоту мира?  
> Честно говоря, я сейчас чувствую только отсутствие http.

<!--
https://ru.wikipedia.org/wiki/%D0%A3%D0%B4%D0%B0%D0%BB%D1%91%D0%BD%D0%BD%D1%8B%D0%B9_%D0%B2%D1%8B%D0%B7%D0%BE%D0%B2_%D0%BF%D1%80%D0%BE%D1%86%D0%B5%D0%B4%D1%83%D1%80
-->
- WIP: [HTTP](protocols/http.md)
- WIP: [HTTP2 (HTTP/2, HTTP/2.0)](protocols/http2.md)
- WIP: [TCP/IP](protocols/tcp-ip.md)
- WIP: [TLS](protocols/tls.md)
- **[WebSocket](protocols/websocket.md)** - Двусторонний обмен сообщениями между клиентом и сервером поверх ТСР соединения.
- **[События, посылаемые сервером (Server-Sent Events, SSE)](protocols/sse.md)** - Односторонние сообщения от сервера к клиенту поверх HTTP соединения.
- WIP: [Длинный опрос (Long Polling)](protocols/long-polling.md)
- WIP: [Короткий опрос (Short Polling)](protocols/short-polling.md)
- WIP: [Джиттер (Jitter)](protocols/jitter.md)
- WIP: [Удалённый вызов процедур (Remote Procedure Call, RPC)](protocols/rpc.md)
  - WIP: [gRPC](protocols/grpc.md)
  - WIP: [tRPC](protocols/trpc.md)

---
## SQL, Базы данных <a name="sql-and-db"></a>

> [!TIP]
> SQL-запрос заходит в бар, подходит к двум столам и спрашивает: "можно присоединиться?"

- WIP: [Нормализация и денормализация](sql-and-db/normalization-and-denormalization.md)
- WIP: [Связь многие ко многим (Many-to-many)](sql-and-db/many-to-many.md)
- WIP: [Связь один ко многим (One-to-many)](sql-and-db/one-to-many.md)
- WIP: [Связь один к одному (One-to-one)](sql-and-db/one-to-one.md)
- WIP: [CRUD](sql-and-db/crud.md)
- WIP: [Шардирование баз данных](sql-and-db/db-sharding.md)
- WIP: [Типы баз данных](sql-and-db/types-of-db.md)
- WIP: [Индексы](sql-and-db/indexes.md)
- **[Транзакции](sql-and-db/transactions.md)** - набор последовательных операций с базой данных, соединенных в одну логическую единицу
  - [Уровень изоляции Read uncommitted](sql-and-db/transactions.md#uncommitted) - доступ к еще не подтвержденным завершением транзакции данным.
  - [Уровень изоляции Read committed](sql-and-db/transactions.md#committed) - доступ только к подтвержденным завершением транзакции данным.
  - [Уровень изоляции Repeatable read или Snapshot isolation](sql-and-db/transactions.md#repeatable-read) - доступ к снепшоту данных созданному в начале транзакции.
  - [Уровень изоляции Serializable](sql-and-db/transactions.md#serializable) - никакого доступа к данным до завершения транзакции.
- WIP: [Соединения с сопоставлениями строк (JOIN) ](sql-and-db/join.md)

### PostgreSQL <a name="sql-and-db-postgresql"></a>
<!--
https://postgrespro.ru/docs/postgrespro/10/tutorial-transactions
https://habr.com/ru/articles/843794/
https://postgrespro.ru/docs/postgrespro/9.6/transaction-iso
https://habr.com/ru/articles/860982/
https://postgrespro.ru/docs/postgresql/13/plpgsql-transactions
https://postgrespro.ru/docs/enterprise/9.6/atx
https://postgrespro.ru/docs/postgresql/9.6/queries-table-expressions
-->
- WIP: [Типы данных](sql-and-db/postgresql/types.md)
- **[Индексы](sql-and-db/postgresql/indexes.md)**
  - [B-дерево (B-tree, Balanced tree)](sql-and-db/postgresql/indexes.md#b-tree)
  - [Хеш (Hash)](sql-and-db/postgresql/indexes.md#hash)
  - [GiST](sql-and-db/postgresql/indexes.md#gist)
  - [SP-GiST](sql-and-db/postgresql/indexes.md#sp-gIst)
  - [GIN](sql-and-db/postgresql/indexes.md#gin)
  - [BRIN](sql-and-db/postgresql/indexes.md#brin)
- WIP: [Транзакции](sql-and-db/postgresql/transactions.md)
- WIP: [Блокировки](blocking.md)
- WIP: [Фильтрация (HAVING)](sql-and-db/postgresql/having.md)
- WIP: [Группировка (GROUP BY)](sql-and-db/postgresql/group-by.md)
- WIP: [Многоуровневая группировка (GROUPING SETS)](sql-and-db/postgresql/grouping-sets.md)
- WIP: [Вычисление итогов (CUBE)](sql-and-db/postgresql/cube.md)
- WIP: [Вычисление итогов (ROLLUP)](sql-and-db/postgresql/rollup.md)
- WIP: [Оконные функции](sql-and-db/postgresql/window-functions.md)
- WIP: [Процедурные функции](sql-and-db/postgresql/procedural-functions.md)
- WIP: [Статистика содержимого таблиц (ANALYZE)](sql-and-db/postgresql/analyze.md)
- WIP: [План выполнения (EXPLAIN)](sql-and-db/postgresql/explain.md)
- **[Освобождение пространства (VACUUM)](sql-and-db/postgresql/vacuum.md)** - Высвобождает пространство, занимаемое "мёртвыми" данными. При параметре ANALYZE обновляет статистику, которую использует планировщик.
- **[Карта видимости](visibility-map.md)** - Внутренние данные, в каких страницах есть только записи, видимые для всех активных и всех будущих транзакций.
- WIP: [Оптимизация](sql-and-db/postgresql/optimization.md)
- WIP: [Полезные приемы](sql-and-db/postgresql/usefull.md)

### MongoDB <a name="sql-and-db-mongodb"></a>
- WIP: [Виды индексов](sql-and-db/mongodb/indexes.md)
- WIP: [Транзакции](sql-and-db/mongodb/transactions.md)

### Redis <a name="sql-and-db-redis"></a>

### Elasticsearch <a name="sql-and-db-elasticsearch"></a>

---
## Брокеры сообщений <a name="message-brokers"></a>

> [!TIP]
> Люди, которые пишут всю свою мысль в одном большом сообщении, вы отбитые? Те кто по одному слову отправляет миллион сообщений - к вам вопросов нет. 

### RabbitMQ <a name="message-brokers-rabbitmq"></a>

### Nats (Neural Autonomic Transport System) <a name="message-brokers-nats"></a>

### Kafka <a name="message-brokers-kafka"></a>
[//]: # (- партиции,)
[//]: # (- не блокирующие обработки)
[//]: # (- хертбиты &#40;хертбиты, хеартбиты&#41;)

---
## Языки программирования <a name="languages"></a>

> [!TIP]
> Работа программиста и шамана имеет много общего - оба бормочут непонятные слова, совершают непонятные действия и не могут объяснить, как оно работает.

### JavaScript <a name="languages-javascript"></a>
- **[JavaScript: Цикл событий (Event loop) и libuv](languages/javascript/event-loop-and-libuv.md)**
- WIP: [JavaScript: Промисы (Promises)](languages/javascript/js-promises.md)

### TypeScript <a name="languages-typescript"></a>
- WIP: [Интерфейсы](languages/typescript/interfaces.md)
- WIP: [Типы](languages/typescript/types.md)

---
## Фреймворки <a name="frameworks"></a>

> [!TIP]
> Тяжелые времена порождают сильных программистов. Сильные программисты создают фреймворки. Фреймворки порождают слабых программистов. Слабые программисты порождают тяжелые времена.

### NestJs <a name="frameworks-nestjs"></a>
<!--
https://habr.com/ru/companies/timeweb/articles/663234
https://habr.com/ru/companies/timeweb/articles/666470/
-->

---
## DevOps <a name="devops"></a>

> [!TIP]
> Здравствуйте, это канал об аниме? Как мне пропатчить KDE2 под FreeBSD?

[//]: # (- Docker)
[//]: # (- Kubernetes)
[//]: # (- ресурсоы)
[//]: # (- service)
[//]: # (- deploy)
[//]: # (- ingress)
[//]: # (- daemonset)
[//]: # (- configmap)

## CI|CD <a name="cicd"></a>

<!--
https://habr.com/ru/companies/otus/articles/754422/
https://www.jetbrains.com/ru-ru/teamcity/ci-cd-guide/
-->
[//]: # (- Blue-Green деплоймент)
[//]: # (- Canary деплоймент)

---
## Мониторинги <a name="monitorings"></a>

> [!TIP]
> Видишь суслика?  
> Нет...  
> А он есть... (c) к/ф "ДМБ"

- WIP: [Мониторинг сервисов](monitorings/services-monitoring.md)

[//]: # (- Grafana)
[//]: # (- Loki)
[//]: # (- Prometheus)

---
## Документирование <a name="documentation"></a>

> [!TIP]
> Джун: Где документация?  
> Тимлид: Я и есть документация.

[//]: # (- OpenAPI)
[//]: # (- Swagger)

[//]: # (доменные модели? может относиться не к этому разделу)
[//]: # (модели данных? может относиться не к этому разделу)
[//]: # (модели предметной области? может относиться не к этому разделу)

---
## Управление кодом <a name="code"></a>

> [!TIP]
> Не повторяйте одну и ту же ошибку в вашем коде снова и снова. Создайте функцию с ней и вызывайте её каждый раз, когда понадобится.

<!--
https://habr.com/ru/companies/avito/articles/680522/
https://bool.dev/blog/detail/git-branching-strategies
+ Git Flow
+ GitLab flow
и т.п.
-->

---
## Управление персоналом <a name="management"></a>

> [!TIP]
> Один монитор - обычный программист, два монитора - продвинутый программист, три монитора - системный программист, четыре монитора - охранник.

- WIP: [Метрики сотрудников](management/employee-metrics.md)

[//]: # (- Фасилитация)
[//]: # (- системный анализ команды)
[//]: # (- методологии и процессы разработки ПО)
[//]: # (- методологии и процессы работы тимлидом)
[//]: # (- типы требований и их иерархия)
[//]: # (- жизненный цикл разработки ПО)
[//]: # (- процессы управления требованиями)
[//]: # (- атрибуты качества требований разрабатываемого решения)
[//]: # (- гибкие методологии)
[//]: # (- особенности работы с требованиями в гибких методологиях)

---
# Вопросы собеседований <a name="tasks"></a>

> [!TIP]
> Есть два способа написать сложную программу: либо сделать ее настолько простой, что будет казаться, что она проста как два плюс два, либо сделать ее настолько сложной, что невозможно найти ошибки

<!--
https://habr.com/ru/articles/770522/
-->

## JavaScript <a name="tasks-javascript"></a>
1. [Найти пересечение двух массивов](tasks/javascript/two-array-intersection.md)
1. [Очистить массив от повторов](tasks/javascript/clean-doubles-from-array.md)
1. [Перевернуть строку](tasks/javascript/revert-string.md)
1. [Порядок выполнения - 1 (var)](tasks/javascript/execution-order-1.md)
1. [Порядок выполнения - 2 (Promise и setTimeout)](tasks/javascript/execution-order-2.md)
1. [Проверить, является ли строка зеркальной](tasks/javascript/is-mirrored-string.md)
1. [Проверить, является ли строка палиндромом](tasks/javascript/is-palindrome-string.md)
1. [Проверка порядка скобок](tasks/javascript/check-brackets.md)
1. [Что выведет функция - 1 (let)](tasks/javascript/what-output-1.md)
1. [Что выведет функция - 2 (let)](tasks/javascript/what-output-2.md)

## SQL <a name="tasks-sql"></a>
1. [Выборка дублирующихся записей](tasks/sql/search-doubles.md)
