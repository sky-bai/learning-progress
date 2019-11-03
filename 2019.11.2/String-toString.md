# java String toString method

toString方法是string对象的一个方法

返回对象本身（对象本身就是一个字符串）



```java
String str = new String("baibaibai");
//创建String对象要传入参数
System.out.ptintln(str.toString());

```



***

# StringBuffer

其实String有关的类都是将字符串传入数组中

再传入String对象中

String是一个类 需要传入的参数 String直接构建一个不可变的对象

```
char data [] = {'a','b','c'};
String str = new String(data);
```

对字符串进行修改需要使用到StringBuffer类



```
StringBuffer sBuffer = new StringBuffer("待传入的值")
```

