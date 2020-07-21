---
title: "[javascript] 산술 연산자"
date: 2020-07-17 14:04:00 -0400
---

## 증가 연산자, 감소 연산자

전위 연산자는 먼저 변수의 값을 바꾼 다음에 평가하고 후위 연산자는 값을 바꾸기 전에 평가한다.

```javascript
let x = 2;
const r1 = x++ + x++;
//          2  +  3
//    r1 = 5, x = 4
const r2 = ++x + ++x;
//          5  +  6
//    r2 = 11, x = 6
const r3 = x++ + ++x;
//          6  +  8
//    r3 = 14, x = 8
const r4 = ++x + x++;
//          9  +  9
//    r4 = 18, x = 10
```

```javascript
let y = 10;
const r5 = y-- + y--;
//          10 +  9
//    r5 = 19, y = 8
const r6 = --y + --y;
//          7  +  6
//    r6 = 13, y = 6
const r7 = y-- + --y;
//          6  +  4
//    r7 = 10, y = 4
const r8 = --y + y--;
//          3  +  3
//    r8 = 6, y = 2
```
