---
title: "[백준] 30319 - Advance to Taoyuan Regional (C++)"
date: 2023-10-31 11:13:36 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/30319>

## 풀이

10월 21일의 35일 전인 9월 16일 이전인지, 이후인지 확인하면 됩니다.

```cpp
#include <iostream>
using namespace std;

int main() {
  string date;
  cin >> date;

  if (date <= "2023-09-16") {
    cout << "GOOD";
  } else {
    cout << "TOO LATE";
  }

  return 0;
}
```
