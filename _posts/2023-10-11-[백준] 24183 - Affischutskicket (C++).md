---
title: "[백준] 24183 - Affischutskicket (C++)"
date: 2023-10-11 10:48:14 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/24183>

## 풀이

약간 헷갈리는 면이 있는 브론즈 4 문제입니다.

```cpp
#include <iostream>
using namespace std;

int main() {
  double C4, A3, A4;
  cin >> C4 >> A3 >> A4;

  cout.precision(6);
  cout << fixed;
  cout << (2 * C4 * 74196 + 2 * A3 * 124740 + A4 * 62370) * 0.000001;

  return 0;
}
```
