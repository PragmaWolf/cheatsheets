# JavaScript. Очистить массив от повторов

Дан массив вида:
```javascript
const test = [0, 2, 3, 4, 2, 5, 3, 4, 0, 3, 6, 8, 1, 9, 7, 1];
```
Необходимо удалить из него все дубли существующих элементов. В результате должен получиться массив вида:
```javascript
const result = cleanDoubles(test); // [0, 2, 3, 4, 5, 6, 8, 1, 9, 7];
```

---

## Решение 1
Оценка алгоритма - **O(2n)**

```javascript
function cleanDoubles(arr) {
  return Array.from(new Set(arr));
};
```

---

## Решение 2
Оценка алгоритма - **O(n^2)**

```javascript
function cleanDoubles(arr) {
  return arr.filter((value, index) => {
    return arr.indexOf(value) == index;
  });
};
```
