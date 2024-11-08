# Библиотека libuv

Библиотека отвечающая за неблокирующие операции и взаимодействие с операционной системой в Node.js.

Для эмуляции неблокирующего ввода/вывода использует внутри потоки (именно в ОС Linux, в других ОС такого нет).

> [!IMPORTANT]
> **В Linux**, на текущий момент, все операции с локальными файлами — блокирующие

**Особенности**
- По-умолчанию поднимаются 4 потока (именно в ОС Linux, в других ОС такого нет).

# Цикл событий (Event Loop)

Механизм Event Loop'a находится в libuv.

В Node.js цикл событий позволяет выполнять неблокирующие операции ввода/вывода путем выгрузки операций в ядро системы, когда это возможно.

Когда одна из этих операций завершается, ядро сообщает Node.js, что соответствующая этой операции функция обратного вызова (коллбэк) может быть добавлена в очередь опроса.

**Упрощённый порядок выполнения операций (фазы):**
- Таймеры (кроме setImmediate).
- I/O коллбэки выполненных операций.
- Ожидание и подготовка (внутренние процессы цикла событий, может быть выполнен только process.nextTick()).
- Опрос (I/O операции, входящие: соединения, данные и т.д. Ставятся ядром в очередь).
  - Сначала выполнение скриптов для таймеров, порог которых истек.
  - Затем обработка событий из очереди опроса.
  - Может простаивать в ожидании задач или таймеров
  - Если в процессе ожидания истек порог таймера - он выполнится.
- Проверка (здесь запускается setImmediate).
- Коллбеки `close`.
- Проверка ожидается ли завершение каких-либо асинхронных операций ввода/вывода или таймеров, и завершает работу, если их нет.

**Особенности:**
Каждая фаза имеет очередь колбеков работающую по принципу FIFO. 
Каждая фаза выполняет сначала операции относящиеся к ней, а затем колбеки из очереди.
Фаза завершается, когда очередь колбеков исчерпана или если обработано максимально допустимое количество колбеков.

## Стек

Вызов любой функции создаёт контекст выполнения (Execution Context). При вызове вложенной функции создаётся новый контекст, а старый сохраняется в специальной структуре данных - стеке вызовов (Call Stack).

Если в рамках выполнения текущей функции (first) вызывается другая функция (second):
- Контекст текущей функции (first) помещается в стек вызовов.
- Новый контекст вызываемой функции (sercond) помещается в стек вызовов выше текущей.
- Когда выполнится вызываемая функция (second) ее контекст удаляется из стека вызовов.
- Выполнение передается контексту текущей функции (first).
- Когда выполняется текущая функция (first) ее контекст так же удаляется из стека вызовов.

## Куча

Содержит таймеры.
Функция-запуска таймеров вытягивает из кучи обработчик таймера с наименьшим временем и сравнивает это значение с временем выполнения событийного цикла. 
В случае, если время таймера меньше, то этот таймер останавливается (удаляется из кучи, его обработчик тоже удаляется из кучи). 
Далее идет проверка, нужно ли его перезапустить.

## Очередь

Это список задач для обработки.

**Особенности**
- Задача по сути является функцией с параметрами.
- Выполнение задачи вызывает ассоциированную с ней функцию, контекст которой в свою очередь помещается в стек вызовов.
- Задача считается выполненной, когда связанный с ней стек вызовов пуст.
- Каждая задача выполняется полностью, прежде чем начнёт обрабатываться следующая.

## process.nextTick()

Сразу помещается в текущий цикл (фазу). 

Будет обрабатываться после завершения текущей операции, независимо от текущей фазы цикла событий.

Когда вызывается `process.nextTick()` на любой фазе, все коллбэки, переданные процессу `process.nextTick()`, будут разрешаться до того, как цикл событий продолжится.

Удобно обращаться к коллбекам в функциях - гарантирует выполнение функции и вызов колбека. 
В частности, если синхронная функция вызывается с асинхронной сигнатурой (await).

**Варианты использования**
- Обрабатывать ошибки, очищать любые ненужные ресурсы или, возможно, повторять попытку до продолжения цикла обработки событий.
- Иногда необходимо разрешить выполнение коллбэка после разбора стека вызовов, но до продолжения цикла событий.

## setImmediate()

Срабатывает на следующей итерации или «тике» цикла событий.

Обработается только в фазе Проверки - выполнится после всех событий ввода/вывода.
