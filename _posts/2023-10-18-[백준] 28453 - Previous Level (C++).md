---
title: "[백준] 28453 - Previous Level (C++)"
date: 2023-10-18 11:40:58 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/28453>

## 풀이

더 큰 숫자의 카드를 가지고 있는것이 절대적으로 유리하므로, 둘 중 더 큰 값을 출력하면 됩니다.

```cpp
#include <iostream>
using namespace std;

int main() {
  int N;
  cin >> N;

  while (N--) {
    int M;
    cin >> M;

    if (M < 250) {
      cout << "4 ";
    } else if (250 <= M && M < 275) {
      cout << "3 ";
    } else if (275 <= M && M < 300) {
      cout << "2 ";
    } else {
      cout << "1 ";
    }
  }

  return 0;
}
```
