
## 题目描述

给出 $n$ 个等腰三角形，每个三角由 $x,y,m$ 三个参数来确定。

这三个参数确定三角形的三个点分别为 $(x,y),(x+m,y)\ and\ (x,y+m)$。

求所有三角形覆盖的总面积。

## 输入格式

第一行一个整数 $n$。

下面 $n$ 行给出 $x_i,y_i,m_i$。

## 输出格式

输出三角形覆盖的总面积，答案保留一位小数。


```input1
5
-5 -3 6
-1 -2 3
0 0 2
-2 2 1
-4 -1 2
```


```output1
24.5
```

## 样例说明

![](file://pic1.jpg)

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n\leq2\times 10^3$，$-10^7\leq x_i,y_i\leq10^7$，$0 < m_i< 10^3$。
