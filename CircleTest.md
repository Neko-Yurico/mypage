# 实验3 一个常见问题的解析
实验3是面向对象实验，对于大家来说有点难度，基本点总结如下。
#
两个java源文件，代表两个类    
`Circle.java`里面写的是
```
public class Circle
```
`CircleTest.java`里面写的是
```
public class CircleTest
```
这是main类

最常见的问题，在`class` 里面再写`class`。像下面这样就是不对的。
```
public class EX03{
	public class Circle{
}
}
```
其实语法上没有问题，Circle是EX03的内部类，但是在实验3中用不到。大家只要记住，一般没有特殊情况，一个文件内部一个类。不要在类中间套类。

