---
title: "[javascript] 구조 분해 할당"
date: 2020-07-20 13:53:00 -0400
---

## 구조 분해 할당

구조 분해 할당 구문은 배열이나 객체의 속성을 해체하여 그 값을 개별 변수에 담을 수 있게 한다.
```javascript
const obj = {b:2, c:3, d:4};
const {a, b, c} = obj;
a;              // undefined
b;              // 2
c;              // 3
d;              // ReferenceError
```

위 예제에서는 선언과 할당을 같은 문에서 실행했다. 객체 해체는 할당만으로 이뤄질 수도 있는데 그렇게 하려면 반드시 괄호를 써야 한다. 괄호를 쓰지 않으면 자바스크립트는 표현식 좌변을 블록으로 해석한다.
```javascript
const obj = {b:2, c:3, d:4};
let a, b, c;
{a, b, c} = obj;   // error
({a, b, c} = obj); // work
```
배열을 해체할 때는 배열 요소에 대응할 변수 이름을 마음대로 쓸 수 있다.
```javascript
const arr = [1, 2, 3];
let [x, y] = arr;
x;              // 1
y;              // 2
z;              // ReferenceError
```