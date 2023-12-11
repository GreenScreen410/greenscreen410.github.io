---
title: "[백준] 14534 - String Permutation (Python)"
date: 2023-12-11 19:28:52 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/14534>

## 풀이

기본적인 백트래킹 문제입니다. 순열을 구해주는 함수가 있는 언어들도 일부 있습니다.

```python
from itertools import permutations

T = int(input())
for i in range(1, T + 1):
    L = input()

    print(f"Case # {i}:")
    for i in permutations(L, len(L)):
        print("".join(i))
```
