## 题目描述

给出一个带权的连通无向图，对于其中的每条边 $i$，在原来边权的基础上，其边权每增加1需要付出的代价为 $a_i$，边权每减少 $1$ 需要付出的代价为 $b_i$，现在指定该图的一棵生成树，求通过修改边权，使得该生成树成为图的一棵最小生成树，需要付出的最少总代价。

## 输入格式

第一行两个正整数 $n, m$，表示图的点数和边数，点以 $1 \sim n$ 编号；
接下来 $m$ 行，每行六个正整数 $u_i, v_i, w_i, ff_i, a_i, b_i$，表示一条边 $(u_i, v_i) $ 权为 $w_i$ ，在原边权基础上增加 $1$ 的边权代价为 $a_i$，减少 $1$ 的边权代价为 $b_i$， $ff_i$ 若为 $1$ 则表示该边在指定的生成树中，若为 $0$ 表示不在。数据保证 $ff$ 值为 $1$
的边刚好组成原图的一棵生成树。两点之间可能有多条不同的边，但没有连接同一点的边。

## 输出格式

输出一个正整数，表示所需付出的最少总代价。



```input1
6 8
1 2 3 1 4 2
1 4 2 0 3 4
2 3 5 1 2 1
2 4 4 1 3 5
3 5 2 0 1 3
3 6 1 0 2 4
4 5 7 1 3 2
5 6 5 1 5 4
```



```output1
21
```

## 样例说明：

最优方案为：$(1, 4) $ 边权加 $2$，代价 $6$；$(3, 5) $ 边权加 $3$，代价 $3$；$(3, 6)$ 边权加 $4$，代价 $8$；$(4, 5)$ 边权减 $2$，代价 $4$；总代价  $21$。

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 300$，$1 \le m, w_i,a_i, b_i \le 10^3$。

