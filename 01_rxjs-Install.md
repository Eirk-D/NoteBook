### p1
RxJS is a library for composing asynchronous and event-based programs by using observable sequences.
It provides one core type, the Observable, satellite types (Observer, Schedulers, Subjects) and operators inspired by
Array#extras (map, filter, reduce, every, etc) to allow handling asynchronous events as collections.  
<把异步事件当做集合来处理>

### p2
ReactiveX combines the Observer pattern with the Iterator pattern and functional programming with collections 
to fill the need for an ideal way of managing sequences of events.
The essential concepts in RxJS which solve async event management are:
<把观察者模式和迭代器模式、函数式编程结合起来以管理一系列的事件>

Observable: represents the idea of an invokable collection of future values or events.  // 可调用的集合
Observer: is a collection of callbacks that knows how to listen to values delivered by the Observable. // 监听Observable传递的值
Subscription: represents the execution of an Observable, is primarily useful for cancelling the execution. // 订阅事件的处理
Operators: are pure functions that enable a functional programming style of dealing with collections // 运算符
with operations like map, filter, concat, reduce, etc.
Subject: is the equivalent to an EventEmitter, and the only way of multicasting a value or event to multiple Observers. // 广播到多个观察者的唯一途径
Schedulers: are centralized dispatchers to control concurrency, allowing us to coordinate when // 调度： 控制并发
computation happens on e.g. setTimeout or requestAnimationFrame or others.
<主要类型有 Observable、Observer、Subscription、Operators、Subject、Schedulers六种类型>
