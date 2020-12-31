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

##stringbuilder
是一个可变的字符串类，可以看做一个容器
构造方法
StringBuilder sb = new StringBuilder(“字符串”)

## append 和reverse

sb.append("字符串") //就可以把括号的内容加入到sb里面
链式拼接: sb.append(1).append(2)....

sb.reverse():可以实现字符串反转

## stringbuilder and string 转换
要用tostring的方法
string s = sb.toString(); stringbuilder给 string
反过来用
stringBuilder sb = new stringBuilder（s）；

可以链式操作
new stringBuilder(s).reverse().toString(); 可以完成对字符串的反转
