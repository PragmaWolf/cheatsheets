**[Вопросы собеседований](../../README.md#tasks) ::**
**[JavaScript](../../README.md#tasks-javascript) ::**
# Что выведет функция - 1 (let)

Дан код:
```javascript
function genArr() {
    const arr = [];

    let i = 0;
    while (i < 10) {
        const func = () => {
            console.log(i);
        }
        arr.push(func);
        i++;
    }

    return arr;
}

const test = genArr();
console.log(test[0]());
console.log(test[5]());
```

Что будет выведено в консоли? 

[К оглавлению](../../README.md#tasks-javascript)

---

## Решение

В консоль выведется:
```
10
10
```

**Объяснение:**
1. Объявление `let i` находится в контексте функции `genArr`.
2. Затем запускается цикл, который заполняет массив анонимными стрелочными (лямбда) функциями.
3. Каждая анонимная стрелочная функция будет выводить `i` в контексте функции `genArr`.
4. По окончании работы цикла `i` примет значение `10` и функция `genArr` отдает массив анонимных функций.
5. При вызове любой анонимной функции из массива будет идти обращение к `i`, в контексте функции `genArr`.
6. Так как  `i` имеет финальное значение `10`, то при вызове любой анонимной функции из массива будет отдаваться `10`.
7. Соответственно в консоли будет выведено 2 строки, каждая из которых будет содержать значение `10`.

[К оглавлению](../../README.md#tasks-javascript)

> [!IMPORTANT]
> Если вы заметили ошибку, неточность, нехватку информации, пожалуйста, сообщите мне.
