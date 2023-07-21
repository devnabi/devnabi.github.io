---
layout: post
title:  "exersize_java01"
image: ''
date:   2023-07-20
tags:
- Kitri - Exersize Java
description: ''
categories:
- Kitri - Exersize Java
---

```java
package exersize_java01;

import java.util.Scanner;

public class Ex01 {

    public static void main(String[] args) {
        // Ex1 : 자신의 이름을 키보드로 입력 받아 콘솔 화면에 출력하는 프로그램을 구현하세요.
        Scanner sc = new Scanner(System.in);
        String name = sc.nextLine();
        System.out.println(name);
    }
}

```

```java
package exersize_java01;

public class Ex02 {

    public static void main(String[] args) {
        // Ex2 : 다음의 코드에서 변수 a와 b의 값을 서로 교환하기 위해 코드를 추가해주세요.

        int a = 10;
        int b = 20;
        int c; // 빈 변수

        c = a;
        a = b;
        b = c;
        System.out.println("a = " + a);
        System.out.println("b = " + b);

    }
}

```

```java
package exersize_java01;

public class Ex03 {

    public static void main(String[] args) {
        // Ex3 : 빈칸에 들어갈 타입은 무엇인지, 출력되는 결과와 그 이유를 설명해보세요.

        int x = 5;
        int y = 2;
        int result = x / y;
        System.out.println(result);
        // 이유 : 결과는 2다. 정수 나누기 정수라서 답도 정수로 출력된다. 나머지 없이 몫만 나오는 연산자다.
    }
}

```

```java
package exersize_java01;

public class Ex04 {

    public static void main(String[] args) {
        // Ex4 : 변수 result가 출력되는 결과로 2.5 가 나오게 하고 싶습니다. 빈칸의 코드를 완성해보세요.
        
        int x = 5;
        int y = 2;
        double result = (double)x / y;
        System.out.println(result);
    }
}

```

```java
package exersize_java01;

public class Ex05 {

    public static void main(String[] args) {
        // Ex5 : var1부터 var4까지 + 연산을 수행해서 int 타입 result 변수에 9가 저장되도록 빈칸의 코드를 완성해보세요.

        long var1 = 2L;
        float var2 = 1.8f;
        double var3 = 2.5;
        String var4 = "3.9";
        double d = Double.parseDouble(var4);
        System.out.println("d = " + d);
        int result = (int)(var2 + var3) + (int)var1 + (int)d;
        System.out.println("result = " + result);
    }
}

```

```java
package exersize_java01;

public class Ex06 {

    public static void main(String[] args) {
        // Ex6 : 문자열 “20230701”을 기본 타입으로 변환하려고 합니다. 반대로 정수형 20230701을 문자열로 변환하려면 어떻게 해야하는지 코드를 작성해보세요.

        // 1. 문자열을 기본 타입으로 변환
        String str = "20230701";
        int result = Integer.parseInt(str);
        System.out.println("문자열을 기본 타입으로 변환 = " + result);

        // 2. 정수형 20230701을 String으로 변환
        int i = 20230701;
        String str2 = String.valueOf(i);
        System.out.println("정수형을 String으로 변환 = " + str2);

    }
}

```

```java
package exersize_java01;

public class Ex07 {

    public static void main(String[] args) {
        // Ex7 : 다음과 같이 출력되도록 주어진 코드를 완성해보세요.
        
        // 이름 : 이강인
        // 나이 : 23
        // 전화 : 010-1111-1234

        // 주어진 코드
        String name = "이강인";
        int age = 23;
        String tel1 = "010", tel2 = "1111", tel3 = "1234";

        // 답
        System.out.println("이름 : "+ name);
        System.out.println("나이 : " + age);
        System.out.println("전화 : " + tel1 + "-"+ tel2 + "-"+ tel3);
    }
}

```

```java
package exersize_java01;

import java.util.Scanner;

public class Ex08 {

    public static void main(String[] args) {
        // Ex8 : Scanner 클래스를 이용해 이름, 주민번호 앞 6자리, 전화번호를 키보드에서 입력받고 출력하는 코드를 작성해보세요.

        // [필수 정보 입력]
        // 1. 이름 : _ (입력받아야함)
        // 2. 주민번호 앞 6자리 : _ (입력받아야함)
        // 3. 전화번호 : _ (입력받아야함)

        //         [입력한 내용]
        // (입력받은 이름)
        // (입력받은 주민번호 앞 6자리)
        // (입력받은 전화번호)

        Scanner sc = new Scanner(System.in);
        String str = sc.nextLine();
        int i = Integer.parseInt(sc.nextLine());
        String str2 = sc.nextLine();

        System.out.println("1. 이름 : " + str);
        System.out.println("2. 주민번호 앞 6자리 : " + i);
        System.out.println("3. 전화번호 : " + str2);

    }
}

```

```java
package exersize_java01;

public class Ex09 {

    public static void main(String[] args) {
        // Ex9 : 다음 코드에서 컴파일 에러가 발생하는 위치와 이유를 설명해보세요. 그리고 컴파일 에러를 없앨 수 있도록 코드를 고쳐보세요.

        // byte b = 5;
        // b = -b;
        // int result = 10 / b;
        // System.out.println(result);

        // 에러나는 이유 : -은 단항 연산자다. 산출결과는 int로 저장해야하기때문에 에러가 난다.

        // 고친 답
        byte b = 5;
        int i = -b;
        int result = 10 / b;
        System.out.println(result);
    }
}

```

```java
package exersize_java01;

public class Ex10 {

    public static void main(String[] args) {
        // Ex10 : 증감 연산자와 덧셈 연산자(+)를 이용해 z의 값이 28이 되도록 코드를 작성해보세요.

        int x = 10;
        int y = 20;
        int z = --x + --y;
        System.out.println(z); // 28이 나와야 한다.
    }
}

```

```java
package exersize_java01;

public class Ex11 {

    public static void main(String[] args) {
        // Ex11 : 다음 코드를 실행하면 출력 결과로 5가 나오길 기대했는데 4가 출력 되었습니다. 어디에서 잘못된 것일까요?

        // 5.0 나누기 2는 실수다. 그래야 2.5가 나와서 * 2 는 5가 된다. double로 바꿔주지 않아서 답은 정수/정수로 4가 나오기때문에 잘못됐다.
        //int var1 = 5;
        //int var2 = 2;
        //double var3 = var1 / var2;
        //int var4 = (int) (var3 * var2);
        //System.out.println(var4);

        // 고쳐본 것
        int var1 = 5;
        int var2 = 2;
        double var3 = (double)var1 / var2;
        int var4 = (int) (var3 * var2); // 2.5 * 2는 5.0으로 실수가 나오기 때문에 형변환을 해주기
        System.out.println(var4); // 5가 나온다.
    }
}

```

```java
package exersize_java01;

import java.util.Scanner;

public class Ex12 {

    public static void main(String[] args) {
        // Ex12 : 키보드로 아이디와 패스워드를 입력 받습니다. 입력 조건으로 이름은 문자열이고 패스워드는 정수입니다(패스워드는 int 타입으로 변환).
        // 입력된 내용을 비교해서 아이디가 “kitri”이고 패스워드가 12345라면 “로그인 성공”을 출력하고 그렇지 않으면 “로그인 실패”를 출력하도록 프로그램을 만들어 보세요.

        Scanner scanner = new Scanner(System.in);

        System.out.print("아이디:");
        String name = scanner.nextLine();

        System.out.print("패스워드:");
        String strPassword = scanner.nextLine();
        int password = Integer.parseInt(strPassword);

        // 이후 로그인 성공인지 실패인지를 체크하는 조건문 작성
        if((name.equals("kitri")) && password == 12345) {
            System.out.println("로그인 성공");
        }
        else {
            System.out.println("로그인 실패");
        }
        // --- Your code here! ---
    }
}

```

```java
package exersize_java01;

import java.util.Scanner;

public class Ex13 {

    public static void main(String[] args) {
        // Ex13 : 사용자로부터 키보드로 점수를 입력받아 점수가 60점 이상이면 “pass” 60점 미만이면 “fail” 을 출력하는 삼항 조건 연산자를 작성해보세요.
        // 3항 연산자 : 조건문 ? 참 : 거짓
        
        Scanner sc = new Scanner(System.in);

        String strScore = sc.nextLine(); // 점수를 입력받는 것이니까 int로 바꿔주기
        int score = Integer.parseInt(strScore);

        // --- your code here ---
        String str = (60 <= score) ? "pass" : "fail";
        System.out.println(str);
    }
}

```
