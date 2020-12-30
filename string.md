## 特点
字符串不可变，创建后无法更改但是可以被共享
相当于cahr[]

## 构造方法 推荐使用直接赋值的方法来创建字符串

public String() = 空白字符串

char[] chs = {'a','b','c'};
String s2 = new String(chs);

byte[] bys = {97,98,99};
String s2 = new String(bys);

String s4 = "abc";

## string对象的特点
new string 每次都会申请一个相同的地址，
但是"" 的方法是会让JVM 建立字符串池，第二次赋值直接参考对象，所以本质是一个对象

