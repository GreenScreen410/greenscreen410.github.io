---
title: "[백준] 2523 - 별 찍기 - 13 (C++)"
date: 2023-10-14 14:35:32 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/2523>

## 풀이

단순 별 찍기 문제입니다. 가운데까지 출력하는 반복문, 그리고 아래 별이 감소하는 부분을 출력하는 반복문 두개가 있습니다.

```cpp
#include <iostream>
using namespace std;

int main() {
  int N;
  cin >> N;

  for (int i = 1; i <= N; i++) {
    for (int j = 1; j <= i; j++) {
      cout << "*";
    }
    cout << "\n";
  }
  for (int i = N - 1; i >= 1; i--) {
    for (int j = 1; j <= i; j++) {
      cout << "*";
    }
    cout << "\n";
  }

  return 0;
}
```
