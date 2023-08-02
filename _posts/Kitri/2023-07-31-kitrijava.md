---
layout: post
title:  "인터페이스"
image: ''
date:   2023-07-31
tags:
- Kitri - Study java
description: ''
categories:
- Kitri - Learn Java
---

```java
package interface07;

public interface RemoteControl{
    int MAX_VOLUME = 10;

    public void turnOn();

    public void turnOff();

    public void setVolume();
}

```

```java
package interface07;

public class AirConditional implements RemoteControl{
    int volume;
    @Override
    public void turnOn() {
        System.out.println("에어컨을 켠다.");
    }

    @Override
    public void turnOff() {
        System.out.println("에어컨을 끈다.");
    }

    @Override
    public void setVolume() {
        System.out.println("볼륨을 설정한다.");
    }
}

```
