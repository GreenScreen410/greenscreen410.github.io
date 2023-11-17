---
title: "[백준] 30658 - Os últimos serão os primeiros (C++)"
date: 2023-11-15 11:40:46 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/30658>

## 풀이

입력되는 배열을 뒤집어서 출력하면 됩니다. 포르투갈어.. 상당히 번역하기 힘드네요..

```cpp
#include <iostream>
#include <vector>
using namespace std;

int main() {
  while (1) {
    int n;
    cin >> n;

    if (n == 0) break;

    vector<int> v(n);
    for (int i = 0; i < n; i++) {
      cin >> v[i];
    }

    for (int i = n - 1; i >= 0; i--) {
      cout << v[i] << "\n";
    }
    cout << "0\n";
  }

  return 0;
}
```
