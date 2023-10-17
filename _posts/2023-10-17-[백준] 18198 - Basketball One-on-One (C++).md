---
title: "[백준] 18198 - Basketball One-on-One (C++)"
date: 2023-10-17 11:08:09 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/18198>

## 풀이

2점을 먼저 앞서야 하는 듀스 상황도 구현해야 할 것 같지만, 맨 마지막에 득점한 사람이 이기므로 고려하지 않아도 됩니다.

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
  string score;
  cin >> score;

  int A = 0, B = 0;
  for (int i = 0; i < score.size(); i += 2) {
    if (score[i] == 'A') A += score[i + 1] - '0';
    else B += score[i + 1] - '0';
  }

  cout << (A > B ? "A" : "B");

  return 0;
}
```
