## 题目描述

给出一个 $n$ 个点 $m$ 条边的无向图，$n$ 个点的编号从 $1-n$，定义源点为 $1$。定义最短路树如下：从源点 $1$ 经过边集 $T$ 到任意一点 $i$ 有且仅有一条路径，且这条路径是整个图 $1$ 到 $i$ 的最短路径，边集 $T$ 构成最短路树。 给出最短路树，求对于除了源点 $1$ 外的每个点 $i$，求最短路，要求不经过给出的最短路树上的 $1$ 到 $i$ 的路径的最后一条边。

## 输入格式

第一行包含两个数 $n$ 和 $m$，表示图中有 $n$ 个点和 $m$ 条边。
接下来 $m$ 行，每行有四个数 $a_i,b_i,l_i,t_i$，表示图中第 $i$ 条边连接 $a_i$ 和 $b_i$ 权值为 $l_i$，$t_i$ 为 $1$ 表示这条边是最短路树上的边，$t_i$ 为 $0$ 表示不是最短路树上的边。

## 输出格式

输出 $n-1$ 个数，第 $i$ 个数表示从 $1$ 到 $i+1$ 的要求的最短路。无法到达输出 $-1$。

```input1
5 9
3 1 3 1
1 4 2 1
2 1 6 0
2 3 4 0
5 2 3 0
3 2 2 1
5 3 1 1
3 5 2 0
4 5 4 0
```

```output1
6 7 8 5
```

## 数据规模与约定

对于 $100\%$ 的数据，$n\le 4000,m\le 100000,1\le li\le 100000$
