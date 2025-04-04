**[Структуры данных](../../README.md#data-structures) ::**
**[Описание структур данных](../../README.md#data-structures-descriptions) ::**
# Кортеж (Tuple)

> [!IMPORTANT]
> Кортежи близки к структурам, но структурами не являются.

Упорядоченный набор фиксированной длины. Неизменяемая последовательность элементов - после создания такой структуры, ее нельзя изменить: добавить, удалить или изменить элементы. Это обеспечивает целостность и предсказуемость данных. Занимают меньше памяти, чем [списки](lists.md), и, как следствие, обеспечивают более быстрый доступ к данным.

Основная идея заключается в объединении нескольких значений в единое целое. Это позволяет сохранять и передавать сразу несколько взаимосвязанных элементов, что значительно упрощает процесс обработки информации.

В языках программирования со статической типизацией кортеж отличается от [списка](lists.md) тем, что элементы кортежа могут принадлежать разным типам и набор таких типов заранее определён типом кортежа, а значит, и размер кортежа также определён. С другой стороны, коллекции ([списки](lists.md), [массивы](arrays.md)) имеют ограничение по типу хранимых элементов, но не имеют ограничения на длину.

В функциональных языках [некаррированные](carrining.md) функции нескольких аргументов принимают параметры в виде одного аргумента, являющегося кортежем.

**Особенности**
- В основном значения в кортежах неименованные, но это зависит от языка программирования (в некоторых можно создавать именованные). 
- В основном доступ к элементам по индексу, но это зависит от языка программирования (в некоторых можно обращаться по имени).
- Невозможность изменять количество элементов.
- Элементы могу быть разных типов.

**Примеры кортежей:**
- Список аргументов функции.
- Список инициализации структуры или массива.
- Список аргументов шаблона или макроса.
- Обычный блок кода (элементами являются не объекты, а синтаксические конструкции).
- Хранение координат точки на плоскости (x, y).

[К оглавлению](../../README.md#data-structures-descriptions)

## В базах данных
В реляционных базах данных кортеж - это, упрощенно, запись (строка) таблицы.

[К оглавлению](../../README.md#data-structures-descriptions)

## Операции

|      Создание      | Вставка |       Обход        | Поиск | Сортировка | Слияние | Обновление |  Удаление  |
|:------------------:|:-------:|:------------------:|:-----:|:----------:|:-------:|:----------:|:----------:|
| :heavy_check_mark: |   :x:   | :heavy_check_mark: |  :x:  |    :x:     |   :x:   | :question: | :question: |

- :heavy_check_mark: - операция доступна.
- :x: - операция **не**доступна.
- :question: - зависит от реализации в языке программирования.

> [!CAUTION]
> Могут быть ошибки в описании операций 

[К оглавлению](../../README.md#data-structures-descriptions)

> [!IMPORTANT]
> Если вы заметили ошибку, неточность, нехватку информации, пожалуйста, сообщите мне.
