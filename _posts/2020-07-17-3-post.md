---
title: "[javascript] 원시 타입과 객체"
date: 2020-07-17 14:04:00 -0400
---

## 원시 타입과 객체

자바스크립트의 값은 원시 값(_primitive_) 또는 객체(_object_)이다. 문자열과 숫자 같은 원시 타입은 불변(_immutable_)이다. 원시 타입에는 여섯 가지가 있다.

- 숫자
- 문자열
- 불리언
- null
- undefined
- 심볼

원시 값과 달리 객체는 여러 가지 형태와 값을 가질 수 있다. 자바스크립트에는 몇 가지 내장된 객체 타입이 있다.

- Array
- Date
- RegExp
- Map, WeakMap
- Set, WeakSet

객체의 본질은 **컨테이너**이다. 내용물은 바뀔 수 있지만 컨테이너는 바뀌지 않는다. 객체의 콘텐츠는 프로퍼티(_property_) 또는 멤버(_member_)라고 부른다. 프로퍼티는 이름(키)과 값으로 구성된다.

```javascript
const me = {
  name: "3people",
  favorite: {
    food: "라면",
    movie: "interstellar",
    game: "LOL",
  }, // 객체가 프로퍼티 값이 될 수 있다.
  greeting: function () {
    console.log("Hello");
  }, // 함수도 프로퍼티 값이 될 수 있다.
};
```
