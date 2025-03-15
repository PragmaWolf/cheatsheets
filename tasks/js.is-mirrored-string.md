**[Вопросы собеседований](../../README.md#вопросы-собеседований) :: [JavaScript](../../README.md#javascript-1) ::**
# Проверить, является ли строка зеркальной

Дана строка:
```javascript
const test = 'a bc def ghijihg fed cb a';
```
Необходимо проверить, является ли эта строка зеркальной, тоесть читаемой одинаково с обеих сторон с учетом всех символов.

Например:
```javascript
isPalindrome('a bb a'); // true
isPalindrome('a bba'); // false
```

[К оглавлению](../README.md#javascript-1)

---

## Решение 1
Оценка алгоритма - **O(n)**

```javascript
function isMirrored(str) {
  let result = true;
  const halfLen = Math.floor(str.length / 2);
  for (let i = 0; i < halfLen; i++) {
    if (str[i] !== str[str.length - 1 - i]) {
      result = false;
      break;
    }
  }
  return result;
};
```

[К оглавлению](../README.md#javascript-1)

---

## Решение 2
Оценка алгоритма - **O(3n)**

```javascript
function isMirrored(str) {
  const reverse = str.split('').reverse().join('');
  return (str === reverse);
};
```

[К оглавлению](../README.md#javascript-1)
