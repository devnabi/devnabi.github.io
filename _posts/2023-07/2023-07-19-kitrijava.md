---
layout: post
title:  "변수와 타입(1)"
image: ''
date:   2023-07-19
tags:
- Kitri - Study java
description: ''
categories:
- Kitri - Learn Java
---

```java
public class Main {

    public static void main(String[] args) {
        // 2023-07-19 - 변수와 타입

        // 메소드가 종료되면 메모리에서 없어진다는 것을 보고 가비지컬렉터를 말하는 것인가 질문했다. 그건 객체만 그런것인가? 변수의 특징인가?
        // 어떻게 동작하는가? : 매소드가 호출되면 스택이 쌓인다. 그러다가 언젠가 종료되면 메모리에 사라진다는 뜻이다.
        // 운영체제를 공부하면 나온다고 한다. 가비지 컬렉터 동작 검색하기

        System.out.println("이주희");

        // SQL과 다르게 대소문자 구분을 꼭 한다. 완전히 다른 변수인 것이다.
        int A = 1;
        int a = 1;

        // 문자열 타입의 변수 선언
        String name = "이주희";
        System.out.println(name);

        // 변수 선언
        int hour = 3;
        int minute = 7;
        System.out.println("Hour = " + hour);
        System.out.println("Minute = " + minute);
        System.out.println(hour + "시간 " + minute + "분"); // 숫자 + 문자열 / 3시간7분

        // 변수 값 재할당
        hour = 4;
        minute = 15;
        System.out.println(hour + "시간 " + minute + "분"); // 4시간 15분
        System.out.println(hour * 60 + minute + "분");

        // 변수의 범위
        int scope = 100;

        {
            int scope2 = 200; // 지역변수
            // 접근이 가능한 것을 확인
            System.out.println(scope);
            System.out.println(scope2);
        }

        // 지역변수가 이 범위에서는 접근이 불가능하다는 것을 확인
        // System.out.println(scope2);
    } // main의 끝
}

```
