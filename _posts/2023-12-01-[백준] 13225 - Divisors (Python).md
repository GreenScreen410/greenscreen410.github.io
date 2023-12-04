---
title: "[백준] 13225 - Divisors (Python)"
date: 2023-12-01 09:20:41 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/13225>

## 풀이

1부터 n까지 반복문을 돌리며, i와 n이 나누어 떨어지는 횟수를 구하면 됩니다.

```python
C = int(input())

for _ in range(C):
    n = int(input())

    divisors = 0
    for i in range(1, n + 1):
        if n % i == 0:
            divisors += 1
    
    print(n, divisors)
```
