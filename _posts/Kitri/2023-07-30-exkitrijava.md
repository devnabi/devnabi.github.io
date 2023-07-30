---
layout: post
title:  "exersize_java02(2)"
image: ''
date:   2023-07-30
tags:
- Kitri - Exersize Java
description: ''
categories:
- Kitri - Exersize Java
---

```java
package exersize_java02;

public class Ex07 {

    public static void main(String[] args) {
        // Ex7 : for문을 이용해서 다음과 같이 * 를 출력하는 코드를 작성해보세요.
        //    *
        //   **
        //  ***
        // ****

        // aaaab / i가 1번째 돌 때 a는 4개
        // aaabb / i가 2번째 돌 때 a는 3개
        // aabbb / i가 3번째 돌 때 b는 3개
        // abbbb / i가 4번째 돌 때 b는 4개
        // bbbbb / i가 4번째 돌 때 b는 5개

        for(int i = 1; i <= 5; i++){
            for(int k = 5; k > i; k--){
                System.out.printf(" ");
            }
            for(int j = 1; j < i; j++){
                System.out.printf("*");
            }
            System.out.println("*");
        } // for의 끝

        // 나중에 언젠간 2번 써서 성공해보기...
        // for(int i = 1; i <= 5; i++){
        //    for(int j = 1; j <= i; j++){
        //        System.out.printf("*");
        //    }
        //    System.out.printf("%n", "*");
    } // main의 끝
}

```

```java
package exersize_java02;

import java.util.Scanner;

public class Ex08 {

    public static void main(String[] args) {
        // Ex8 : while문과 Scanner를 이용해서 키보드로 입력된 데이터로 예금, 출금, 조회, 종료 기능을 제공하는 코드를 작성해보세요.
        // 프로그램을 실행하면 Result 같은 실행결과가 나와야 합니다. (Scanner의 nextLine() 메소드 사용)

        // 예금액 - depositAmount
        // 출금액 - withdrawalAmount
        // 잔고 - accountBalance

        boolean run = true;
        int balance = 0; // 잔고
        String depositAmount = ""; // 예금액
        String withdrawalAmount = ""; // 출금액

        Scanner sc = new Scanner(System.in);

        // 종료조건 걸기 : break;
        while (run) {
            System.out.println("-------------------------------------");
            System.out.println("1.예금 | 2.출금 | 3.잔고 | 4.종료");
            System.out.println("-------------------------------------");
            System.out.printf("선택 : ");
            String choice = sc.nextLine();
            if(choice.equals("1")){
                System.out.printf("예금액 : ");
                String str = sc.nextLine();

                depositAmount = str;
                int de = Integer.parseInt(depositAmount); // 예금
                balance += de;
                continue;
            }
            if (choice.equals("2")) {
                System.out.printf("출금액 : ");
                String str = sc.nextLine();

                withdrawalAmount = str;
                int wi = Integer.parseInt(withdrawalAmount); // 출금
                balance -= wi;
                continue;
            }
            if (choice.equals("3")) {
                System.out.println("잔고 : " + balance);
            }
            if(choice == "4"){
                break;
            } //--- write your core here ---
        } // while의 끝
        System.out.println("프로그램 종료"); // while문을 빠져나오면 출력하는 것
    } // main의 끝
}

```

```java
package exersize_java02;

public class Ex09 {

    public static void main(String[] args) {
        // Ex9 : 4개의 정수값 가운데 최댓값을 구하여 출력하는 int max4(int a, int b, int c, int d) 메소드를 작성해주세요.

        // 호출
        System.out.println(max4(10, 9, 5, 2));
    } // main의 끝

    // 메서드 작성
    public static int max4(int a, int b, int c, int d){
        // 실습5의 예시를 참고해서 해보기

        // 변수 선언
        int max = a;

        // 비교하기
        if(max < b){
            max = b;
        }
        if(max < c){
            max = c;
        }
        if(max < d){
            max = d;
        }
        return max;
    }
//    public static int max4(int a, int b, int c, int d){
//        // 내가 해본 것...그냥 비교하기
//        if(a > b && a > c && a > d){
//            return a;
//        }
//        else if(b > a && b > c && b > d){
//            return b;
//        }
//        else if(c > a && c > b && c > d){
//            return b;
//        }
//        else {
//            return d;
//        }
//    } // 메서드의 끝
}

```

```java
package exersize_java02;

public class Ex10 {

    public static void main(String[] args) {
        // Ex10 : 3개의 정수값 가운데 중앙값을 구하여 출력하는 int med3(int a, int b, int c) 메소드를 작성해주세요.

        // 호출
        System.out.println(med3(2, 100, 10));
    } // main의 끝

    // 메서드 작성
    public static int med3(int a, int b, int c){
        int median = a;

        if(a >= b && a <= c){
            return median = a;
        }
        if(b >= a && b <= c){
            return median = b;
        }
        if(c >= a && c <= b){
            return median = c;
        }
        return median;
    }
}

```

```java
package exersize_java02;

public class Ex11 {

    public static void main(String[] args) {
        // Ex11 :  1~10의 합은 (1 + 10) * 5와 같이 구할 수 있습니다.
        // 이를 ‘가우스의 덧셈’이라고 하는데 이 방법을 이용하여 1부터 n까지의 정수 합을 구하는 프로그램을 작성하세요.

        // System.out.println((1 + n) * n / 2);

        // 호출
        System.out.println(Sum1(10));

//        for(int i = 1; i <= n; i++){
//            sum += i;
//        }
//        System.out.println(sum);
    } // main의 끝

    // 메서드 작성
    public static int Sum1(int n){
        return (1 + n) * n / 2;
    }
}

```

```java
package exersize_java02;

import java.util.Scanner;

public class Ex12 {

    public static void main(String[] args) {
        // Ex12 : * 을 n개 출력하되 w개마다 줄 바꿈을 하는 프로그램을 만들어 보세요.
        // *를 n개 출력하되 w개마다 줄을 바꿔서 출력합니다.
        // n값: 14 // <- 14는 사용자가 입력
        // w값: 5 // <- 5는 사용자가 입력
        // *****
        // *****
        // ****

        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        int w = sc.nextInt();
        System.out.println("n값 : " + n);
        System.out.println("w값 : " + w);

        for(int i = 0; i < n; i++){
            if(i % w == 0){
                System.out.println();
            }
            System.out.printf("*");
        } // for의 끝

        // 호출
        // Star(14, 5);
    } // main의 끝

//    // 메서드 작성
//    public static void Star(int n, int w){
//        for(int i = 1; i <= n; i++){
//            if(i % w == 1){
//                System.out.printf("%n");
//            }
//            System.out.printf("*");
//        } // for의 끝
//    } // 메서드의 끝
}

```

```java
package exersize_java02;

public class Ex13 {

    public static void main(String[] args) {
        // Ex13 : n단의 피라미드를 출력하는 메소드를 작성하세요.
        // [4단 예시]
        //	 *
        //  ***
        // *****
        //*******

        // 1단일 때 >> *1개
        // 2단일 때 >> *3개
        // 3단일 때 >> *5개
        // 4단일 때 >> *7개
        // 일단은 1번돌 때마다 *이 2개씩 증가하는 반복문 해보기?

        // 1단일 때 >> 왼 공백이 3개
        // 2단일 때 >> 왼 공백이 2개
        // 3단일 때 >> 왼 공백이 1개
        // 4단일 때 >> 왼 공백이 0개
        // 오른쪽도 마찬가지. 왼 공백개수 * 2를 한 것이 한줄 총 공백 수
        // 공백이 줄어드는 반복문 해보기

        // 호출
        pyramid(4);
    } // main의 끝

    // 메서드 작성
    public static void pyramid(int n){
        for(int i = 0; i < n; i++){
            for(int k = n - 1; k > i; k--){
                System.out.printf(" ");
            } // 공백 1개씩 없애기

            for(int j = 0; j < i; j++){
                System.out.printf("**");
            } // *이 2개씩 증가하는 반복문
            System.out.println("*"); // 개행하며 n단까지 반복 출력
        } // for의 끝
    }
}

```

```java
package exersize_java02;

public class Ex14 {

    public static void main(String[] args) {
        // Ex14 : n단의 숫자 피라미드를 출력하는 메소드를 작성하세요.
        // [5단 예시]
        //	  1
        //   222
        //  33333
        // 4444444
        //555555555

        // 호출
        Numpyramid(5);
    } // main의 끝

    // 메서드 작성
    public static void Numpyramid(int n){
        // 1. 먼저 1부터 5까지 출력하는 반복문을 쓰기
        // 2. 공백 차감하는 반복문 쓰기
        for(int i = 1; i <= n; i++){
            for(int j = n - 1 ; j >= i; j--){
                System.out.printf(" ");
            }
            for(int k = 1; k < i; k++){
                System.out.printf("%d", i);
                System.out.printf("%d", i);
            }
            System.out.println(i);
        } // for의 끝
    } // 메서드의 끝
}

```

```java
package exersize_java02;

import java.util.Scanner;

public class Ex15 {

    public static void main(String[] args) {
        // Ex15 : 1~100까지 랜덤 숫자 맞히기 게임
        // <게임 규칙>
        //
        // * 임의의 숫자를 생성한다. (1~100의 임의의 랜덤 정수)
        // * 다음 과정을 10회 반복한다.
        //    1. 플레이어로부터 숫자를 입력받는다.
        //    2. 입력 받은 숫자가 임의의 숫자와 일치한다면 축하 메시지를 출력하고 반복문 탈출
        //    3. 입력 받은 숫자가 임의의 숫자보다 작다면 작다는 메시지 출력
        //       입력 받은 숫자가 임의의 숫자보다 크다면 크다는 메시지 출력
        //  10번의 기회가 지날 동안 숫자를 맞추지 못하면 게임은 종료된다.

        Scanner sc = new Scanner(System.in);

        // 임의의 랜덤숫자
        int randomNum = (int)(Math.random() * 100) + 1;

        // 기회
        int turn = 0;

        // 1. 플레이어로부터 숫자 입력 받기

        // false일 때 까지 반복하라는 조건을... 뭐가 10이하일 때까지 반복해.
        while (++turn <= 10) {
            int num = sc.nextInt();
            if(num == randomNum){
                System.out.println("정답! 축하합니다~");
                return;
            }
            if(num < randomNum){
                System.out.println("입력하신 숫자는 정해진 숫자보다 작습니디.");
            }
            if(num > randomNum){
                System.out.println("입력하신 숫자는 정해진 숫자보다 큽니다.");
            }
        } // while의 끝
    } // main의 끝
}

```
