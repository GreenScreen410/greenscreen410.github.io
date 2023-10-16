---
title: "[백준] 15128 - Congruent Numbers (Python)"
date: 2023-10-16 16:17:20 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/15128>

## 풀이

크기를 구한 뒤, 정수로 변환했을 때와 일치하는지 확인하면 됩니다.

```python
p1, q1, p2, q2 = map(int, input().split())
size = p1 / q1 * p2 / q2 / 2

if int(size) == size:
    print("1")
else:
    print("0")
```
