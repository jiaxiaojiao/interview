# 同步与异步
Java中交互方式分为同步和异步两种：

- 同步交互

    指发送一个请求,需要等待返回或者轮训去查看是否完成,然后才能够发送下一个请求，有个等待过程；
    
    如果数据将在线程间共享。例如正在写的数据以后可能被另一个线程读到，或者正在读的数据可能已经被另一个线程写过了，那么这些数据就是共享数据，必须进行同步存取。
    
    银行的转账系统，对数据库的保存操作等都会使用同步交互操作。

- 异步交互

    指发送一个请求,不需要等待返回,随时可以再发送下一个请求，即不需要等待。
    
    当应用程序在对象上调用了一个需要花费很长时间来执行的方法，并且不希望让程序等待方法的返回时，就应该使用异步编程，在很多情况下采用异步途径往往更有效率。

区别：一个需要等待，一个不需要等待，在部分情况下，我们的项目开发中都会优先选择不需要等待的异步交互方式。




