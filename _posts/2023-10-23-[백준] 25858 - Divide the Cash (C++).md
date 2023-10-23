---
title: "[백준] 25858 - Divide the Cash (C++)"
date: 2023-10-23 09:15:55 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/25858>

## 풀이

비례배분을 구현해야 하는 문제입니다.

```cpp
#include <iostream>
#include <numeric>
#include <vector>
using namespace std;

int main() {
  int n, d;
  cin >> n >> d;

  vector<int> v(n);
  for (int i = 0; i < n; i++) {
    cin >> v[i];
  }
  int sum = accumulate(v.begin(), v.end(), 0);
  int reward = d / sum;

  for (int i = 0; i < n; i++) {
    cout << v[i] * reward << "\n";
  }

  return 0;
}
```
