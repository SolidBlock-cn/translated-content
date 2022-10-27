---
title: Math.tan()
slug: Web/JavaScript/Reference/Global_Objects/Math/tan
tags:
  - JavaScript
  - Math
  - Method
  - Reference
translation_of: Web/JavaScript/Reference/Global_Objects/Math/tan
---
{{JSRef("Global_Objects", "Math")}}

## Сводка

Метод **`Math.tan()`** возвращает тангенс числа.

## Синтаксис

```
Math.tan(x)
```

### Параметры

- `x`
  - : Число, представляющее угол в радианах.

## Описание

Метод `Math.tan()` возвращает числовое значение, представляющее тангенс угла.

Поскольку метод `tan()` является статическим методом объекта `Math`, вы всегда должны использовать его как `Math.tan()`, а не пытаться вызывать метод на созданном экземпляре объекта `Math` (поскольку объект `Math` не является конструктором).

## Примеры

### Пример: использование метода `Math.tan()`

```js
Math.tan(1); // 1.5574077246549023
```

Поскольку метод `Math.tan()` принимает радианы, а чаще проще работать с градусами, следующая функция принимает значение в градусах, преобразует их в радианы и возвращает тангенс.

```js
function getTanDeg(deg) {
  var rad = deg * Math.PI/180;
  return Math.tan(rad);
}
```

## Спецификации

| Спецификация                                                         | Статус                   | Комментарии                                            |
| -------------------------------------------------------------------- | ------------------------ | ------------------------------------------------------ |
| ECMAScript 1-е издание.                                              | {{Spec2('ES1')}}     | Изначальное определение. Реализована в JavaScript 1.0. |
| {{SpecName('ES5.1', '#sec-15.8.2.18', 'Math.tan')}} | {{Spec2('ES5.1')}} |                                                        |
| {{SpecName('ES6', '#sec-math.tan', 'Math.tan')}}     | {{Spec2('ES6')}}     |                                                        |

## Совместимость с браузерами

{{Compat}}

## Смотрите также

- {{jsxref("Math.acos()")}}
- {{jsxref("Math.asin()")}}
- {{jsxref("Math.atan()")}}
- {{jsxref("Math.atan2()")}}
- {{jsxref("Math.cos()")}}
- {{jsxref("Math.sin()")}}