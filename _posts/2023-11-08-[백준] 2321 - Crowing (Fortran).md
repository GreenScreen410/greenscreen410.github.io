---
title: "[백준] 2321 - Crowing (Fortran)"
date: 2023-11-08 14:00:22 +0900
categories: [Algorithm, BOJ]
tags: []
---

## 문제

<https://www.acmicpc.net/problem/2321>

## 풀이

찾아보니 * 방식으로 출력하면 '알아서 적당한 방식'으로 출력해서, 출력 형식 오류가 발생한다고 하네요..? 😓

```fortran
program Main
  print '(a)', ",~"
  print '(a)', "( 9> //)"
  print '(a)', " )(_///"
  print '(a)', "( \_>/"
  print '(a)', " \__/"
  print '(a)', "  ^^"
 
  stop
end program Main
```
