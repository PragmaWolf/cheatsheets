**[Структуры данных](../../README.md#data-structures) ::** 
**[Описание структур данных](../../README.md#data-structures-descriptions) ::**
# Очереди (Queues)

Линейная динамическая коллекция однотипных элементов без фиксированной длины.

- Формат (тип): не фиксированный
- Размер: динамический
- Расположение в памяти: динамическое
- Упорядоченность: последовательная
- Привязка к другим элементам: к последующему и/или предыдущему

**Особенности**
- Работа по принципу FIFO (First In, First Out).
- Быстрый доступ к первому элементу.
- Не позволяют произвольный доступ к другим элементам.
- Приоритетная очередь:
  - У каждого элемента присутствует приоритет.
  - Выбирается для обработки элемент с максимальным приоритетом.
  - После обработки элемент с максимальным приоритетом удаляется из очереди.
  - Возможность изменения приоритета.
  - Возможна организация такой очереди с помощью структуры данных Куча (heap).

**Операции:**
- Создание: да
- Вставка: да
- Обход: нет
- Поиск: нет
- Сортировка: нет
- Слияние: нет
- Обновление: нет
- Удаление: да

[К оглавлению](../../README.md#data-structures-descriptions)
