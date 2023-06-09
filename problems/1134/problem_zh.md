## 题目描述

在三角形图上，每个小正三角形的面积都是 $1$。可以在边上走出一个多边形，（即三角形网格图的边界，见下图）使得围成一定的面积。 我们可以用编码来表示走法：（即从一条边到下一条边的方向改变量） $a$ 左转 $120°$，$b$ 左转$60°$，$c$ 直走，$d$ 右转$60°$，$e$ 右转 $120°$，可以描述为 `cdddcddd` 或 `dddcdddc`，`cbbbcbbb`。对于描述同样形状的图形的不同序列，我们只用字典序最小的，即 `bbbcbbbc` 两个多边形在几何的概念上全等即看做等价。显然等价的图形用字母路径表示出来是一样的。 你的任务有两个： 

1. 对于给定的N输出所有面积为N的可以走出来的图形的编码 
2. 对于给定的形状序列，求出其面积K并计算在这个图形基础上加一个小三角形可以组成哪些可编码图形。 

数据保证 $N,K \le 10$。

## 输入格式

第一行数据总数 $t$。

每个询问以 `N` 开头则表示任务 1，接下来一个整数 $N$。以 `K` 开头则表示任务 2，接下来是一个字符串。

## 输出格式

对于每个任务，输出两行， 第一行表示满足要求的方案总数。

第二行按字典序输出所有序列，两个序列之间用一个空格隔开。

```input1
2
K adeccecced
N 5
```

```output1
5
acedccecced addebcecced adebebecced adecbedcced cceccecce
4
aeddde bdecdde bececde ccedcde
```

## 数据规模与约定

$t \le 5$。

$N,K \le 10$。