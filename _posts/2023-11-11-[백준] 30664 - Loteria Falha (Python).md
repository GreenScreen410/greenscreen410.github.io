---
title: "[백준] 30664 - Loteria Falha (Python)"
date: 2023-11-08 11:19:10 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/30664>

## 풀이

42로 나누어 지는지 확인하면 되지만.. 자릿수가 최대 30이므로 큰 수 연산을 해야 합니다.

```python
while True:
    n = int(input())
    if n == 0:
        break
    
    if n % 42 == 0:
        print('PREMIADO')
    else:
        print('TENTE NOVAMENTE')
```
