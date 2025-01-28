---
id: "[C] perror"
aliases:
  - "[C] perror"
tags:
  - C
  - stdio.h
---
# [C] perror

## Intro

```C
#include <stdio.h>

void
perror(const char *s);
```

## Description

- 전역변수 `errno` 에 현재 저장되어 있는 값에 해당하는 에러 메세지를 찾아서 표준 에러로 출력. (개행 포함)
- 매개변수 `s`에 `null`이 아닌 문자열이 주어지는 경우 콜론과 공백(`": "`) 으로 구분해서 에러 메세지와 함께 출력.
- 에러 번호에 해당하는 에러 메세지가 없는 경우 `Unknown error: <에러 번호>` 를 출력.

## Resources

- [man perror]()

