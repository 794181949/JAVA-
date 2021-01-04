## File类
file是文件和目录路径名的抽象表示，可以用file封装成对象
File(String, Sring child); 或者直接pathname
File f1 = new File("E:\\itcast\\java.txt");

或者
File(file,String child);


file 类的功能
createNewFile() 文件不存在可以创建空文件
eg sout(f1.creatNewFile()); 

mkdir() 创建目录 : 如果目录不存在就创建目录返回true
f2.mkdir()

mkdirs() 创建多级目录包括不存在的父目录

方法不同调用出来的结果也不一样，一个是文件，一个是目录，如果用相同名字的目录，同名字的文件无法创建

## 判断和获取功能
isDirector(), isFile(), exists()
getAbsoluPath()得到绝对路径字符串
, getPath路径字符串
, getName()文件或目录的名称
, list()在文件路径表示的目录中的文件和目录的名称字符串数组,
listFiles()文件和目录的名称file对象数组  -  可以根据文件类型来判断

## 删除功能
delete() = 可以删除目录或者文件

绝对路径：是完整的路径，不需要其他信息就可以定位，E:\\glo\\love.txt
相对路径：必须取自其他路径名的信息进行解释 eg myLove\\glo.txt

f1.delete(), f2.delete()
注意，删除目录，如果目录里面有文件，是无法删除的，因此先删除里面的内容
最后在删除目录

## 递归

    public static int f(int n){
      if (n == 1 || n ==2){
        return 1;
      } else {retrun f(n-1) + f(n-2)}
    }

要找到递归出口和递归规则





