---
layout: single
title:  "C# Static, Namespace"
categories: c#
tag: [c#, static, namespace]
toc: true
toc_sticky: true
author_profile: false
sidebar:
    nav: "docs"
search: true
---

# Static(정적멤버)

## 정의
정적 메서드는 인스턴스 메서드와 다르게 클래스로부터 객체의 생성없이(new 타입을 거치지 않는다) 직접 호출하는 [클래스.메서드명]형식이다.

### 예시
정적 필드
```c#
class Field_Ex{
    static public string name; //정적필드
}
class Program{
    static void Main(){
        Console.WriteLine(Field_Ex.name);
    }
}
```
정적 메서드
```c#
class Method_Ex{
    static public string name; 

    static public void Method(){//정적메서드
        Console.WriteLine(name);
    }
}
class Program{
    static void Main(){
        Method_Ex.Method();
    }
}
```
정적 생성자
주로 정적멤버 초기화하는데 사용
```c#
public static class Class_Ex{    

    public string name = 이름;

    public void Name(){|
        Console.WriteLine(name);
    }

    static Person(){//최초접근 1회만
        Console.WriteLine(name+2);
    }
}
class Program{
    static void Main(){
        Class_Ex ex = new Class_Ex();
        Console.WriteLine("   ");
        Class_Ex ex2 = new Class_Ex();
    }
}
```
정적클래스결과
이름
이름2
   
이름

# Namespace(네임스페이스)

## 정의
네임스페이스는 이름이 중복되어 정의된 것을 구분해주기 위한 것이다.
먼저 .NET은 다음과 같이 네임스페이스를 사용하여 여러 클래스를 구성합니다.
두번째로 많은 클래스를 분류하는 방법으로 사용하고있다.


