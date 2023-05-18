## 题目描述

给定 $K$ 种化学物质和 $N$ 种反应类型。每个反应都有一些反应物和生成物，且反应需要一定的时间。假设每次反应后的若干生成物都可以完全分离。而每次反应的生成物，可以立即用于其他反应的生成物。每种物质的数量都是无限的。

给出一些已有的物质，求得到一种指定物质至少要多少时间。

## 输入格式

第一行包含 $4$ 个整数，分别为 $K$，$N$，已有物质数量 $M$ 和所求物质的编号；

下面依次是 $N$ 种反应的描述。每种反应的描述有三行。第一行包含一个正整数，表示该反应的时间；第二行第一个数是这个反应的反应物的数量，接着是这些反应物的编号；第三行第一个数是生成物的数量，接着是生成物的编号。

已有物质的编号总是 $1$ 到 $M$，编号为 $M+1$ 到 $K$ 的为开始时没有的物质。

## 输出格式

包含一个非负整数，表示生成指定的物质需要的最短的时间。如果无法生成指定物质，则输出 `-1`。

## 样例输入
```plain
4 3 1 4
8
1 1
1 4
3
1 1
2 2 3
2
2 1 3
1 4
```
## 样例输出
```plain
5
```
## 样例说明

依次进行反应二和反应三，可以得到所有种类的物质，耗时为 $5$。

## 数据规模与约定

$30\%$ 的数据满足，$1\le K,N\le 10$；

$100\%$ 的数据满足，$1\le K\le 250，1\le N\le 500$。