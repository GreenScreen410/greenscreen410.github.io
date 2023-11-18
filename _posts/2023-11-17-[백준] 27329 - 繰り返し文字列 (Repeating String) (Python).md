---
title: "[백준] 27329 - 繰り返し文字列 (Repeating String) (Python)"
date: 2023-11-17 11:06:42 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/27329>

## 풀이

문자열을 반으로 나누고, 서로 같은지 다른지 확인하면 됩니다. N이 짝수만 나오고 특별히 고려해야 할 부분이 없으므로 간단히 해결할 수 있습니다.

```python
N = int(input())
S = input()

if S[:N // 2] == S[N // 2:]:
    print('Yes')
else:
    print('No')
```
