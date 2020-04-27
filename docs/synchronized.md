# synchronized使用

synchronized有两种加锁方式：

1、作用于某个实例对象

可以防止多个线程访问这个对象的synchronized同步方法

> 并且一个对象有多个synchronized方法，只要一个线程访问了其中的一个synchronized方法，其它线程不能同时访问这个对象中任何一个synchronized方法。

此外，不同对象实例的synchronized方法是不相干预的。也就是说，其它线程可以同时访问此类下的另一个对象实例中的synchronized方法；

2、作用域某个类上

此作用域下，可以防止多个线程同时访问这个类中的synchronized方法。也就是说此种修饰，可以对此类的所有对象实例起作用。

**注意：synchronized关键字是不能继承的**

。。。。未完待续