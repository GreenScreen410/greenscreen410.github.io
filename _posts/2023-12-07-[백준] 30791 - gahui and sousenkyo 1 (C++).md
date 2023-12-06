---
title: "[백준] 30791 - gahui and sousenkyo 1 (C++).md"
date: 2023-12-07 08:23:23 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/30791>

## 풀이

첫번째 값(16위)과 차가 1000 이하인 것의 개수를 세면 됩니다.

```cpp
#include <iostream>
using namespace std;

int main() {
  int lv;
  string judge;
  cin >> lv >> judge;

  if (judge == "miss") {
    cout << lv * 0;
  } else if (judge == "bad") {
    cout << lv * 200;
  } else if (judge == "cool") {
    cout << lv * 400;
  } else if (judge == "great") {
    cout << lv * 600;
  } else {
    cout << lv * 1000;
  }

  return 0;
}
```
