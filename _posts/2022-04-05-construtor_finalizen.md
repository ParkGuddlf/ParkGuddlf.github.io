---
layout: single
title:  "C# Construtor_Finalizen"
categories: c#
tag: [c#, construtor, finalizen]
toc: true
toc_sticky: true
author_profile: false
sidebar:
    nav: "docs"
search: true
---

# Construtor(생성자)

## 정의
클래스에 객체를 생성하는 역할입니다.
클래스를 선언할 때 생성자를 구현하지 않아도 자동으로 생성자를 만들어줍니다.
클래스에 생성자 메서드를 추가하면 자동으로 객체가 생성되는 시점에 해당 메서드가 호출됩니다.

### 예시
```c#
class construtor{
    static void Main(string[] arg){
        Console.WriteLine("test 객체생성전");
        Test.test = new Test():
        Console.WriteLine("test 객체생성후");
    } 
}
class Test{
    string name;
    public test(){
        name = "확인";
        Console.WriteLine("Test name은 확인");
    }
}
```
결과
test 객체생성전
Test name은 확인
test 객체생성후

# Finalizen(종료자)

## 정의
가비지 컬렉터가 객체의 소멸시점을 판단하여 종료자를 호출한다.
시점을 정확히 판단할 수 없어서 가급적 사용을 하지않는다.

종료자는 클래스 이름 앞에 ~를 붙이면 됩니다.
### 예시
```c#
class Test{
    ~test(){
        //자원 해체를 위한 코드
    }
}
```