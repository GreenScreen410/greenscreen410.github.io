---
title: "[백준] 26350 - Good Coin Denomination (C++)"
date: 2023-10-16 15:43:51 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/26350>

## 풀이

다음 원소가 이전 원소보다 2배 이상인지 계속 확인하면 됩니다.

```cpp
#include <iostream>
#include <vector>
using namespace std;

int main() {
  int n;
  cin >> n;

  while (n--) {
    int d;
    cin >> d;

    vector<int> v(d);
    for (int i = 0; i < d; i++) {
      cin >> v[i];
    }

    cout << "Denominations: ";
    for (int i = 0; i < d; i++) {
      cout << v[i] << " ";
    }
    cout << "\n";

    bool isGood = true;
    for (int i = 1; i < d; i++) {
      if (v[i] < 2 * v[i - 1]) {
        isGood = false;
        break;
      }
    }

    if (isGood) {
      cout << "Good coin denominations!\n\n";
    } else {
      cout << "Bad coin denominations!\n\n";
    }
  }

  return 0;
}
```
