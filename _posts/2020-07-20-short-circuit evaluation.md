---
title: "[javascript] 단축 평가"
date: 2020-07-20 11:44:00 -0400
---

## 단축 평가   

x && y 와 같은 AND 연산을 수행할 때 x가 거짓 같은 값(*falsy*)이면 y의 값을 평가할 필요도 없이 false가 된다. OR 연산도 마찬가지이다. 이런 동작을 단축 평가(*short-circuit evaluation*)라고 한다.

단축 평가가 중요한 이유는 두 번째 피연산자에 부수 효과가 있다 하더라고 단축 평가를 거치면 그 효과는 일어나지 않기 때문이다.

```javascript
const doIt = false;
let x = 0;
const result = doIt && x++;
```
위 코드의 세 번째 행에서 단축 평가가 일어나므로 x의 값은 변하지 않아 0을 유지한다.