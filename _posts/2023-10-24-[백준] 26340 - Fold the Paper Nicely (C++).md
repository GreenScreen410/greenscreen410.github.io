---
title: "[백준] 26340 - Fold the Paper Nicely (C++)"
date: 2023-10-24 11:47:13 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/26340>

## 풀이

매번 둘 중 더 큰 값을 2로 나누면서 진행하면 됩니다.

```cpp
#include <iostream>
using namespace std;

int main() {
  int n;
  cin >> n;

  while (n--) {
    int a, b, count;
    cin >> a >> b >> count;

    cout << "Data set: " << a << " " << b << " " << count << "\n";
    while (count--) {
      if (a > b) {
        a /= 2;
      } else {
        b /= 2;
      }
    }

    cout << max(a, b) << " " << min(a, b) << "\n\n";
  }

  return 0;
}
```
