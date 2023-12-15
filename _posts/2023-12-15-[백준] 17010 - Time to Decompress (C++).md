---
title: "[백준] 17010 - Time to Decompress (C++)"
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/17010>

## 풀이

간단한 반복문 연습 문제입니다.

```cpp
#include <iostream>
using namespace std;

int main() {
  int L;
  cin >> L;

  while (L--) {
    int N;
    string x;
    cin >> N >> x;

    for (int i = 0; i < N; i++) {
      cout << x;
    }
    cout << "\n";
  }

  return 0;
}
```
