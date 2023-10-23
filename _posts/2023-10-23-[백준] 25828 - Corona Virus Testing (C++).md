---
title: "[백준] 25828 - Corona Virus Testing (C++)"
date: 2023-10-23 10:19:30 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/25828>

## 풀이

예제를 직접 풀어보면 조금 더 쉽게 접근할 수 있습니다.

```cpp
#include <iostream>
using namespace std;

int main() {
  int g, p, t;
  cin >> g >> p >> t;

  int one = g * p;
  int group = t > 0 ? p * t + g : g;

  if (one > group) {
    cout << "2";
  } else if (one < group) {
    cout << "1";
  } else {
    cout << "0";
  }

  return 0;
}
```
