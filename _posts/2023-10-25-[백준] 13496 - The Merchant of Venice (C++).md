---
title: "[백준] 13496 - The Merchant of Venice (C++)"
date: 2023-10-25 12:53:39 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/13496>

## 풀이

s와 d의 곱이 최대로 이동할 수 있는 거리입니다. 이것이 $v_i$ 이상이라면 결과에 $d_i$를 더해줍니다.

```cpp
#include <iostream>
using namespace std;

int main() {
  int K;
  cin >> K;

  for (int i = 1; i <= K; i++) {
    int n, s, d;
    cin >> n >> s >> d;

    int result = 0;
    for (int j = 0, di, vi; j < n; j++) {
      cin >> di >> vi;
      if (s * d >= di) result += vi;
    }
    cout << "Data Set " << i << ":\n" << result << "\n" << "\n";
  }

  return 0;
}
```
