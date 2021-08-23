---
title:  "자비스 1주차"

toc: true
toc_sticky: true

categories:
  - C  
tags:
  - [Baekjoon, Array]

date: 2021-06-28

---

## 첫 번째 활동 
```c
#include <stdio.h>

int main(void) {
    
    int scores[9];
    
    for (int i = 0; i < 9; i++) {
        scanf("%d", &scores[i]);
    }
    
    int max = scores[0];
    for (int i = 0; i < 9; i++) {
        if (scores[i] > max)
        {
            max = scores[i];
        }
    }
    printf("%d\n", max);
    

    for (int i = 0; i < 9; i++) {
        if (scores[i] == max)
        {
            printf("%d", i + 1);
        }
    }
    return 0;
}
```
