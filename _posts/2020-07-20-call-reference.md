---
title: "[javascript] 호출과 참조"
date: 2020-07-20 16:17:00 -0400
---

## 호출과 참조   

자바스크립트에서는 함수도 객체이다. 다른 객체와 마찬가지로 넘기거나 할당할 수 있다. 함수 식별자 뒤에 괄호를 쓰면 함수 바디를 실행하고 괄호를 쓰지 않으면 다른 값과 마찬가지로 함수를 참조하는 것이며 그 함수는 실행되지 않는다.

```javascript
function hungry(){
    return "I'm hungry";
}

hungry();               // "I'm hungry"
hungry;                 // function hungry()
```

함수를 호출하지 않고 참조하기만 할 수 있는 특징을 이용해 함수를 변수에 할당해 다른 이름으로 호출할 수 있다.

```javascript
const f = hungry;
f()                     // "I'm hungry"
```

함수를 객체 프로퍼티에도 할당할 수 있다.

```javascript
const obj = {};
obj.f = hungry;
obj.f();                // "I'm hungry"
```

배열도!

```javascript
const arr = [1, 2, 3];
arr[1] = hungry;
arr[1]();               // "I'm hungry"
```