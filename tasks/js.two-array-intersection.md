**[Вопросы собеседований](../README.md#tasks) ::** 
**[JavaScript](../README.md#tasks-javascript) ::**
# Найти пересечение двух массивов

Даны два массива, произвольной длины и содержания. Например:
```javascript
const arr1 = [4, 9, 5, 3, 1, 8, 3, 2];
const arr2 = [9, 4, 9, 8, 4];
```
Опишите алгоритм поиска одинаковых элементов (пересечения) этих двух массивов. Если значение встречается в обоих массивах `arr1` и `arr2` оно должно оказаться в результирующем массиве. Например:
```javascript
const result = [9, 4, 8];
```

[К оглавлению](../README.md#tasks-javascript)

---

## Решение 1
Оценка алгоритма - **O(m*n)**

```javascript
const intersection = (arrOne, arrTwo) => {
    const result = [];
    for (let i = 0; i < arrOne.length; i++) {
        let j = 0;
        let r = 0;
        while (arrTwo[j] !== arrOne[i] && j < arrTwo.length) {
            j++;
        }
        if (j < arrTwo.length) {
            while (result[r] !== arrTwo[j] && r < result.length) {
                r++;
            }
        }
        if (j < arrTwo.length && r === result.length) {
            result.push(arrOne[i]);
        }
    }

    return result;
};
```

[К оглавлению](../README.md#tasks-javascript)

---

## Решение 2
Оценка алгоритма - **O(n+m+(n*m))**

```javascript
const intersection = (arr1, arr2) => {
    const set1 = new Set(arr1);
    const set2 = new Set(arr2);

    return Array.from(set1.intersection(set2))
};
```

[К оглавлению](../README.md#tasks-javascript)
