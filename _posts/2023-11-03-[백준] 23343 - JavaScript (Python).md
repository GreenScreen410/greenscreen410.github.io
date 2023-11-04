---
title: "[백준] 23343 - JavaScript (Python)"
date: 2023-11-03 10:00:02 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/20053>

## 풀이

알고리즘에서 잘 쓰이지는 않지만, 개발할 때 자주 쓰이는 try, catch(except) 문법에 대해 알아볼 수 있는 좋은 문제입니다.

```python
try:
    x, y = map(int, input().split())
    print(x - y)
except ValueError:
    print("NaN")
```
