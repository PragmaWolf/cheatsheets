**[Вопросы собеседований](../../README.md#tasks) ::** 
**[JavaScript](../../README.md#tasks-javascript) ::**
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

[К оглавлению](../../README.md#tasks-javascript)

---

## Решение 1
Оценка алгоритма - **O(n)**

```javascript
function isMirrored(str) {
  // вычиляем длину половины строки
  // если длина строки нечетная, округляем в меньшую сторону, так как центральный символ не должен попадать в проверку - он всегда одинаков
  const halfLen = Math.floor(str.length / 2);
  // перебираем символы первой половины строки 
  for (let i = 0; i < halfLen; i++) {
    // если текущий символ строки не совпадает с символом с конца строки с учетом смещения (i) - возвращаем FALSE
    if (str[i] !== str[str.length - 1 - i]) {
      return false;
    }
  }
  // обработка всей строки завершена и алгоритм не был прерван - возвращаем TRUE
  return true;
};
```

[К оглавлению](../../README.md#tasks-javascript)

---

## Решение 2
Оценка алгоритма - **O(3n)**

```javascript
function isMirrored(str) {
  // переводим исходную строку в массив
  // переворачиваем массив
  // соединяем все значения массива обратно в строку
  const reverse = str.split('').reverse().join('');
  // возвращаем результат сравнения исходной и перевернутой строк
  return (str === reverse);
};
```

[К оглавлению](../../README.md#tasks-javascript)
