---
title: "[javascript] map, filter"
date: 2020-07-24 14:24:00 -0400
---

## map

`map`은 배열 요소를 변형한다. 일정한 형식의 배열을 다른 형슥으로 바꿀 때 유용하다. `map`과 `filter` 모두 사본을 반환하며 원래 배열은 바뀌지 않는다.

```javascript
const cart = [ 
    { name: "Cheese", price: 10 }, 
    { name: "Beer", price: 20 }
];
const names = cart.map(x => x.name);                // ["Cheese", "Beer"]
const prices = cart.map(x => x.price);              // [10, 20]
const discountPrices = prices.map(x => x * 0.5);    // [5, 10]
```

## filter
`filter`는 배열에서 필요한 것들만 남긴다. 어떤 요소를 남길지 판단할 함수를 넘긴다.

```javascript
const numbers = [1, 2, 3, 4, 5];
numbers.filter(x => x < 3);     // [1, 2]
```