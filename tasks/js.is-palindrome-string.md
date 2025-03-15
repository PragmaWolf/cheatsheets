**[Вопросы собеседований](../README.md#tasks) :: [JavaScript](../README.md#tasks-javascript) ::**
# Проверить, является ли строка палиндромом

> Палинтром - это слово или фраза, которые одинаково читаются слева направо и справа налево.

Дана строка:
```javascript
const test = 'А роза упала на лапу Азора';
```
Необходимо проверить, является ли эта строка палиндромом:
```javascript
isPalindrome('А роза упала на лапу Азора'); // true
isPalindrome('Мама мыла раму'); // false
```

[К оглавлению](../README.md#tasks-javascript)

---

## Решение 1
Оценка алгоритма - **O(3n)**

```javascript
function isPalindrome(str) {
  let result = true;
  let source = str.replace(/\s+/gmi, '').toLowerCase();
  const halfLen = Math.floor(source.length / 2);
  for (let i = 0; i < halfLen; i++) {
    if (source[i] !== source[source.length - 1 - i]) {
      result = false;
      break;
    }
  }
  return result;
};
```

[К оглавлению](../README.md#tasks-javascript)

---

## Решение 2
Оценка алгоритма - **O(5n)**

```javascript
function isPalindrome(str) {
  let source = str.replace(/\s+/gmi, '').toLowerCase();
  const reverse = source.split('').reverse().join('');
  return (source === reverse);
};
```

[К оглавлению](../README.md#tasks-javascript)
