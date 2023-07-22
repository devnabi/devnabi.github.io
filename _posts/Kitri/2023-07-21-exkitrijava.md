---
layout: post
title:  "exersize_java02"
image: ''
date:   2023-07-21
tags:
- Kitri - Exersize Java
description: ''
categories:
- Kitri - Exersize Java
---

```java
package exersize_java02;

public class Ex01 {

    public static void main(String[] args) {
        // Ex1 : for문을 이용해서 1부터 100까지 정수 중 3의 배수의 총합을 구하는 코드를 작성해보세요.
        // 실행하면 1683이 나와야 한다.

        int sum = 0;
        for(int i = 1; i <= 100; i++){
            if(i % 3 == 0){
                sum += i;
            }
        } // for의 끝
        System.out.println(sum);
    } // main의 끝
}

```

```java
package exersize_java02;

public class Ex02 {

    public static void main(String[] args) {
        // Ex2 : 중첩 for문을 이용하여 방정식 4x + 5y = 60의 모든 해를 구해서 (x, y) 형태로 출력해보세요. 단, x와 y는 10 이하의 자연수입니다.

        for(int x = 1; x <= 60; x++){
            for(int y = 1; y <= 60; y++){
                if(4 * x + 5 * y == 60 && x <= 10 && y <= 10){
                    System.out.println("(" + x + "," + y + ")");
                }
            }
        } // for의 끝

    } // main의 끝
}

```

```java
package exersize_java02;

public class Ex03 {

    public static void main(String[] args) {
        // Ex3 : 주어진 정수가 양수인지 음수인지 판별하는 void judgeSign(int num) 메소드를 작성해보세요.
        // 양수를 입력한 경우 : 입력하신 값은 양수 입니다.
        // 음수를 입력한 경우 : 입력하신 값은 음수 입니다.

        // 매서드 호출
        judgeSign(-1);


    } // main의 끝

    // 매서드 작성
    public static void judgeSign(int num){
        if(num >= 0){
            System.out.println("입력하신 값은 양수 입니다.");
        }
        else {
            System.out.println("입력하신 값은 음수 입니다.");
        }
    }
}

```

```java
package exersize_java02;

public class Ex04 {

    public static void main(String[] args) {
        // Ex4 : 정수 a, b를 포함하여 그 사이의 모든 정수의 합을 구하여 반환하는 메소드를 작성하세요.

        intSum(1, 5); // 그 사이의 모든 정수의 합? 1에서부터 5까지의 합 : 1 + 2 + 3 + 4 + 5 = 15가 출력되어야 한다.
    } // main의 끝

    // 매소드 작성
    public static void intSum(int a, int b){
        int sum = 0;
        for(int i = a; i <= b; i++){
            sum = sum + i;
        }
        System.out.println(sum);
    } // 매소드의 끝
}

```

```java
package exersize_java02;

public class Ex05 {

    public static void main(String[] args) {
        // Ex5 : 3개의 정수값 가운데 최댓값을 구하여 출력하는 int max3(int a, int b, int c) 메소드를 작성해주세요.
        // System.out.println(max(1, 3, 5)); 최댓값 : 5가 출력되어야 한다.

        // 매서드 호출
        System.out.println(intMax(2, 8, 3)); // 8이 나와야 한다.

    } // main의 끝

    // 매소드 작성
    public static int intMax(int a, int b, int c){
        if(b < a && a > c){
            return a;
        }
        else if (a < b && b > c){
            return b;
        }
        else {
            return c;
        }

    } // 매소드의 끝
}

```

```java
package exersize_java02;

public class Ex06 {

    public static void main(String[] args) {
        // Ex6 : for문을 이용해서 다음과 같이 * 를 출력하는 코드를 작성해보세요.
        // *
        // **
        // ***
        // ****

        for(int i = 1; i <= 5; i++){
            for(int j = 1; j < i; j++){
                System.out.printf("*");
            }
            System.out.println("*");
        } // for의 끝
    } // main의 끝
}

```
