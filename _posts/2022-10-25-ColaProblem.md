---
layout: post
title: 프로그래머스 — 콜라 문제
subtitle : 프로그래머스 — 콜라 문제
tags: [algorithm]
author: Nayeong Kim
comments : False
---


# 프로그래머스 — 콜라 문제

```jsx
function solution(a, b, n) {
  let answer = 0;
  let amount = n; //현재 가지고 있는 빈병의 총 개수

  let remain = 0;

  for (let i = 0; ; i++) {
    let divide = parseInt(amount / a); //몫 계산

    if(divide === 0){
      if(remain === 0){
        return answer;
      }
      else{
        amount = amount + remain;
        remain =0;
        continue;
      }
    }

    remain = remain + (amount % a); //남은 병 추가

    let newColaBottle = divide * b; //받은 new콜라병 개수

    answer = answer + newColaBottle;

    amount = newColaBottle; //받은 new콜라를 다 마실때
  } //나머지 사용

}
```

- 다른 사람 풀이

```jsx
solution = (a, b, n) => Math.floor(Math.max(n - b, 0) / (a - b)) * b
```

- 다른 사람 풀이

```jsx
function solution(a, b, n) {
    let result = 0;

    while (n/a >= 1) {
        let newBottles = Math.floor(n/a)*b;
        result += newBottles;
        n = n%a;
        n += newBottles;
    }

    return result;
}
```