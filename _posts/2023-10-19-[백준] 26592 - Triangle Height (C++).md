---
title: "[백준] 26592 - Triangle Height (C++)"
date: 2023-10-19 10:59:35 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/26592>

## 풀이

더 큰 숫자의 카드를 가지고 있는것이 절대적으로 유리하므로, 둘 중 더 큰 값을 출력하면 됩니다.

```cpp
#include <iostream>
using namespace std;

int main() {
  int n;
  cin >> n;

  while (n--) {
    int c, p;
    cin >> c >> p;

    cout << c << " " << p << "\n";
    cout << (c - 1) * (p - 2) + p << "\n";
  }

  return 0;
}
```
