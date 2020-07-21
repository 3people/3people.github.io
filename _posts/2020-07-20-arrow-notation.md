---
title: "[javascript] 화살표 표기법"
date: 2020-07-20 17:40:00 -0400
---

## 화살표 표기법

화살표 표기법은 function이라는 단어와  중괄호 숫자를 줄이기 위해 고안된 단축 문법이다. 화살표 함수는 항상 익명이다.

화살표 함수에는 세 가지 단축 문법이 있다.
- function을 생략해도 된다.
- 함수에 매개변수가 단 하나 뿐이라면 괄호도 생략할 수 있다.
- 함수 바디가 표현식 하나라면 중괄호와 return 문도 생략할 수 있다.

```javascript
const f1 = function() { return "Hello!"; }
const f1 = () => "Hello!";

const f2 = function(name) { return `Hello, ${name}!`; }
const f2 = name => `Hello, ${name}!`;

const f3 = function(a, b) { return a + b; }
const f3 = (a, b) => a + b;
```