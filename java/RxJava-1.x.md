---
title: RxJava
date: 2017-06-09 10:22:23
categories:
- Music
tags:
- Music
---


# RxJava基本概念
* Observable: 可观察者，即被观察者
* Observer: 观察者，即订阅者
* subscribe: 订阅。
* 事件:
其中:
* Observable和Observer通过subscribe()方法实现订阅关系。从而Observable可以在需要的时候发出事件来通知Observer。






# Observer
```java
Observer<String> observer = new Observer<String>() {
    @Override
    public void onCompleted() {
        System.out.println("Completed");
    }

    @Override
    public void onError(Throwable e) {
        e.printStackTrace();
    }

    @Override
    public void onNext(String s) {
        System.out.println(s);
    }
};
```

