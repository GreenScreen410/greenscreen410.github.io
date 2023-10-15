---
title: "[백준] 26731 - Zagubiona litera (C++)"
date: 2023-10-15 16:13:46 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/26731>

## 풀이

A의 아스키 코드 65부터 Z의 아스키 코드 90까지 반복문을 돌면서, 없는 문자를 탐색하면 됩니다. find 함수는 값을 못 찾았을 경우, 맨 마지막 원소를 반환합니다.

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
  string S;
  cin >> S;

  for (int i = 65; i <= 90; i++) {
    if (find(S.begin(), S.end(), (char)i) == S.end()) {
      cout << (char)i;
    }
  }

  return 0;
}
```
