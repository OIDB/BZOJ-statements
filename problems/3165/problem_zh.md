## 题目描述
要求在平面直角坐标系下维护两个操作：
1. 在平面上加入一条线段。记第 $i$ 条被插入的线段的标号为 $i$。
2. 给定一个数 $k$，询问与直线 $x = k$ 相交的线段中，交点纵坐标最大的线段的编号。

## 输入格式
输入的第一行是一个整数 $n$，代表操作的个数。

接下来 $n$ 行，每行若干个用空格隔开的整数，第 $(i + 1)$ 行的第一个整数为 $op$，代表第 $i$ 次操作的类型。

若 $op = 0$，则后跟一个整数 $k$，代表本次操作为查询所所有与直线 $x = (k + lastans - 1) \bmod 39989 + 1$ 相交的线段中，交点纵坐标最大的线段编号。

若 $op = 1$，则后跟四个整数 $x_0, y_0, x_1, y_1$，记 $x_i' = (x_i + lastans - 1) \bmod 39989 + 1$ ，$y_i' = (y_i + lastans - 1) \bmod 10^9 + 1$。本次操作为插入一条两端点分别为 $(x_0', y_0')$，$(x_1',y_1')$ 的线段。

其中 $lastans$ 为上次询问的答案，初始时，$lastans = 0$。

## 输出格式
对于每次查询，输出一行一个整数，代表交点纵坐标最大的线段的编号。若不存在任何一条线段与查询直线有交，则输出 $0$；若有多条线段与查询直线的交点纵坐标都是最大的，则输出编号最小的线段，同时 $lastans$ 也应更新为编号最小的一条线段。

```input1
6
1 8 5 10 8
1 6 7 2 6
0 2
0 9
1 4 7 6 7
0 5
```
```output1
2
0
3
```

## 数据规模与约定
对于 $100\%$ 的数据，保证 $1 \leq n \leq 10^5,1 \leq k, x_0, x_1 \leq 39989,1 \leq y_0, y_1 \leq 10^9$。