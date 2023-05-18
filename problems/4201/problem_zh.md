## 题目描述

有一类特殊的多边形我们把它称为直角多边形，指的是该多边形的每一个内角都为 $90^\circ$ 或 $270^\circ$，即每一个角都是直角。

表示一个直角多边形的一种方法是使用多边形序列，多边形序列含两种元素：`L` 表示 $90^\circ$、`R` 表示 $270^\circ$。从直角多边形的任意一个角开始，以逆时针的顺序对角进行顺序排列，绕一圈后所得到的序列便是多边形序列。比如正方形的序列为 `LLLL`，而如下图所示的图形可表示为 `LLRLLRLLRLLR`。显然，一个直角多边形有多种表示序列，而一个序列也对应着多个直角多边形。

![](https://hydro.org.cn/d/bzoj/p/4201/file/pic1.JPG)

对于一个直角多边形，如果存在一个多边形内的点，使得从这个点可以看到多边形边上的每一个点，我们认为这个直角多边形是「可观察的」。现在对于给定的序列长度 $n$，请问有多少个序列长度为 $n$ 的不同的多边形序列，满足它所代表的所有直角多边形中，存在一个「可观察的」直角多边形。

## 输入格式

包含一个正整数 $n$。

## 输出格式

包含一个正整数，表示种数。

## 样例
```input1
6
```
```output1
6
```
## 数据规模与约定

对于 $100\%$ 的数据，$n \le 10^{10^5}$。