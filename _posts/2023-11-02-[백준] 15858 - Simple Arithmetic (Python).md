---
title: "[백준] 15858 - Simple Arithmetic (Python)"
date: 2023-11-02 08:46:04 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/15858>

## 풀이

C언어 계열에서는 double을 사용하면 50점, long double을 사용하면 75점, 문자열로 입력받아 한 자리씩 계산하면 100점을 받습니다.
Decimal을 사용하면 문자열로 바꿔 계산할 것 없이, 쉽게 해결할 수 있습니다.

```python
from decimal import Decimal
a, b, c = map(Decimal, input().split())
print("{:.6f}".format(a * b / c))
```
