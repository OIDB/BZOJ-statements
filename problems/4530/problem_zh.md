


## 题目描述
小强要在N个孤立的星球上建立起一套通信系统。这套通信系统就是连接N个点的一个树。
这个树的边是一条一条添加上去的。在某个时刻，一条边的负载就是它所在的当前能够
联通的树上路过它的简单路径的数量。
例如，在上图中，现在一共有了5条边。其中，(3,8)这条边的负载是6，因
为有六条简单路径2-3-8,2-3-8-7,3-8,3-8-7,4-3-8,4-3-8-7路过了(3,8)。
现在，你的任务就是随着边的添加，动态的回答小强对于某些边的负载的
询问。
## 输入格式
第一行包含两个整数N,Q，表示星球的数量和操作的数量。星球从1开始编号。
接下来的Q行，每行是如下两种格式之一：
A x y 表示在x和y之间连一条边。保证之前x和y是不联通的。
Q x y 表示询问(x,y)这条边上的负载。保证x和y之间有一条边。
1≤N,Q≤100000
## 输出格式
对每个查询操作，输出被查询的边的负载。

```input1
8 6
A 2 3
A 3 4
A 3 8
A 8 7
A 6 5
Q 3 8

```

```output1
6
```

## 提示
没有写明提示
## 题目来源
鸣谢佚名上传

