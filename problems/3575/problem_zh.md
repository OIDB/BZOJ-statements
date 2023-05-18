## 题目描述

A 国有 $n$ 座城市，依次标为 $1$ 到 $n$。同时，在这 $n$ 座城市间有 $m$ 条单向道路，每条道路的长度是一个正整数。现在，A 国交通部指定了一条从城市 $1$ 到城市 $n$ 的路径，并且保证这条路径的长度是所有从城市 $1$ 到城市 $n$ 的路径中最短的。不幸的是，因为从城市 $1$ 到城市 $n$ 旅行的人越来越多，这条由交通部指定的路径经常发生堵塞。

现在 A 国想知道，这条路径中的任意一条道路无法通行时，由城市 $1$ 到 $n$ 的最短路径长度是多少。


## 输入格式

第一行是三个用空格分开的正整数 $n,m$ 和 $l$，分别表示城市数目、单向道路数目和交通部指定的最短路径包含多少条道路。

接下来 $m$ 行，每行三个用空格分开的整数 $a$，$b$ 和 $c$，表示存在一条由城市 $a$ 到城市 $b$ 的长度为 $c$ 的单向道路。

这 $m$ 行的行号也是对应道路的编号，即其中第 $1$ 行对应的道路编号为 $1$，第 $2$ 行对应的道路编号为 $2$，$\cdots$，第 $m$ 行对应的道路编号为 $m$。同时，在这
最后一行为 $l$ 个用空格分开的整数 $sp_1,sp_2,\cdots,sp_l$ 依次表示从城市 $1$ 到城市 $n$ 的由交通部指定的最短路径上的道路的编号。


## 输出格式

$l$ 行，每行为一个整数，第 $i$ 行（$i=1,2,\cdots,l$）的整数表示删去编号为 $sp_i$ 的道路后从城市 $1$ 到城市 $n$ 的最短路径长度。

如果去掉后没有从城市 $1$ 到城市 $n$ 的路径，则输出 $-1$。

```input1
4 5 2
1 2 2
1 3 2
3 4 4
3 2 1
2 4 3
1 5
```

```output1
6
6
```

## 数据规模与约定

对于 $100\%$ 的数据满足 $2<n<10^5$，$1<m<2\times 10^5$。所用道路长度大于 $0$ 小于 $10^4$。

数据已加强 `By Vfleaking`。