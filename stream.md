## stream流
配合lamabda来配合stream来过滤操作 list.stream().filter()

## 生成方式
生成list.stream():

collection 可以用默认方法来生成

map体系只能间接生成流， map.keyset().stream; map.values().stream(); map.entrySet().stream();

数组可以用静态of方法， Stream.of(数组）；



中间操作 filter()

list.stream().filer(s -> startsWith("z")).forEach(system.out::println);

limit(size): 截取前指定个数的数据

sikp(long n);跳过指定个数参数，然后返回剩余元素组成流

limit可以和skip配合，可以先跳过然后把剩下的前几个输出

concat(stream a, stream b) 可以连接两个流 是一个静态方法

distinct() 返回由该流的不同元素，组成的流，这样就不会有重复的流






终结操作 forEach()

