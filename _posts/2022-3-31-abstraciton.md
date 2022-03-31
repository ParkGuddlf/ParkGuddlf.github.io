---
layout: single
title:  "C# Abstraciton"
categories: c#
tag: [c#, abstraciton]
toc: true
toc_sticky: true
author_profile: false
sidebar:
    nav: "docs"
search: true
---
# Abstraciton

## 정의
공통된 속성, 기능을 묶어 붙이는것, 이름만 알고 있어도 사용하는데 불편함이 없어야 된다.

### 예시
```c#
int absoulteValue = abs(-5);
printf(absoulteValue);

public class Example{
    public void Move(){
        printf("움직이중");
    }
}
public class Example2{

    int Value(int a){
        printf("입력한값은" + a + "입니다")
    }
}
public class Main {

    public void main() {
        Example ex1 = new Example();
        Example2 ex2 = new Example2();       

        ex1.move();
        ex2.move();
    }
}
```
## 정리
예시와 같이 함수의 이름을 보고 사용법을 알 수 있게 정리해놓은 것들 또는 집적 정리한 것들이다.
