# JavaScript. Перевернуть строку

Дана строка:
```javascript
const test = 'Мама мыла раму';
```
Необходимо перевернуть эту строку задом наперед, чтобы получилась строка вида:
```javascript
const result = reverseString(test); // 'умар алым амаМ';
```

[К оглавлению](../README.md)

---

## Решение 1
Оценка алгоритма - **O(n)**

```javascript
function reverseString(str) {
  let result = '';
  for (let i = str.length - 1; i >= 0; --i) {
    result += str[i];
  }
  return result;
};
```

[К оглавлению](../README.md)

---

## Решение 2
Оценка алгоритма - **O(3n)**

```javascript
function reverseString(str) {
  return str.split('').reverse().join('');
};
```

[К оглавлению](../README.md)
