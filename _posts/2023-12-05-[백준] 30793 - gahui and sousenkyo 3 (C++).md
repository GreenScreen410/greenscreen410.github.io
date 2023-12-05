---
title: "[백준] 30793 - gahui and sousenkyo 3 (C++)"
date: 2023-12-05 11:57:07 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/30793>

## 풀이

지문에 있는 조건문을 그대로 구현하면 됩니다.

```cpp
#include <iostream>
using namespace std;

int main() {
  double p, r;
  cin >> p >> r;

  double v = p / r;
  if (v < 0.2) {
    cout << "weak";
  } else if (0.2 <= v && v < 0.4) {
    cout << "normal";
  } else if (0.4 <= v && v < 0.6) {
    cout << "strong";
  } else {
    cout << "very strong";
  }

  return 0;
}
```
