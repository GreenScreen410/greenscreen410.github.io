---
title: "[백준] 11121 - Communication Channels (C++)"
date: 2023-10-24 11:09:21 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/11121>

## 풀이

결국 두 문자열이 같은지, 다른지 비교하는 문제입니다..

```cpp
#include <iostream>
using namespace std;

int main() {
  int T;
  cin >> T;

  while (T--) {
    string A, B;
    cin >> A >> B;

    bool isSame = true;
    for (int i = 0; i < A.size(); i++) {
      if (A[i] != B[i]) {
        isSame = false;
        break;
      }
    }

    if (isSame) {
      cout << "OK\n";
    } else {
      cout << "ERROR\n";
    }
  }

  return 0;
}
```
