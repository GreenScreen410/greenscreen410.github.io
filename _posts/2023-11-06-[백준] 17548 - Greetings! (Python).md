---
title: "[백준] 17548 - Greetings! (Python)"
date: 2023-11-06 09:35:03 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/17548>

## 풀이

e의 개수를 2배 하여 출력하면 됩니다. heeeeey! 👋

```python
hey = input()
print('h', end='')
for _ in range(hey.count('e') * 2):
    print('e', end='')
print('y')
```
