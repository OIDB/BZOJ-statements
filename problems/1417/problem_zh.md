## 题目描述

给出无向图 G(V,E)。每次操作任意加一条非自环的边(u,v)，每条边的选择是等概率的。问使得 G 连通的期望操作次数。(|V| <= 30, |E| <= 1000)

## 输入格式

第一行两个整数 $N,M（1<=N<=30，0<=M<=1000）$ 接下来 M 行，每行两个整数 X,Y 表示两者之间已修好一条道路。两点之间可以不止修了一条路，也有可能 M 条路已使 N 个点成为一个整体。

## 输出格式

输出一个小数，表示新修道路条数的期望值，保留六位小数。

```input1
4 2
1 2 
3 4
```

```output1
1.500000
```

## 提示

没有写明提示。

## 题目来源

没有写明来源。

