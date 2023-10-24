---
title: "[백준] 29823 - Pakirobot Manhattanis (C++)"
date: 2023-10-24 16:19:32 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/29823>

## 풀이

다양한 풀이 방법이 있습니다. 저는 각 방향으로 이동한 횟수를 모두 구하고, 최댓값과 최솟값을 구하여 서로 빼는 방법을 사용하였습니다.

```cpp
#include <iostream>
using namespace std;

int main() {
  int N;
  cin >> N;

  string move;
  cin >> move;

  int n = 0, e = 0, s = 0, w = 0;
  for (int i = 0; i < N; i++) {
    if (move[i] == 'N') {
      n++;
    } else if (move[i] == 'E') {
      e++;
    } else if (move[i] == 'S') {
      s++;
    } else {
      w++;
    }
  }

  cout << max(n, s) - min(n, s) + max(e, w) - min(e, w);

  return 0;
}
```
