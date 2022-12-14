---
layout: post
title: 에라토스테네스의 체
subtitle : 에라토스테네스의 체에 대해서 알아보자
tags: [algorithm]
author: Nayeong Kim
comments : False
---


# 에라토스테네스의 체

## 에라토스테네스의 체 란?

- 소수를 판별하는 알고리즘
- 다량의 소수를 정확하고 빠르게 판별 가능하다.

---

### 원리

- 배열을 생성하여 초기화
- 2부터 시작해서 특정 수의 배수에 해당하는 수를 모두 지운다.(지울 때 자기자신은 지우지 않고, 이미 지워진 수는 건너뛴다.)
- 2부터 시작하여 남아있는 수를 모두 출력한다.

```jsx

var prime = new Array(end)
    
    for(let i=0; i<=end;i++){
        prime[i] = i;
    }
// 배열 0으로 초기화

    for(let i=2;i<=end;i++) {
        if(prime[i]==0) continue; // 이미 지워진 수라면 건너뛰기

        // 이미 지워진 숫자가 아니라면, 그 배수부터 출발하여, 가능한 모든 숫자 지우기
        for(let j=2*i;j<=end; j+=i) {
            prime[j] = 0;
        }
    }

```

> prime이라는 배열에서 소수가 아닌 index에 해당하는 값들은 전부 0이다.
>