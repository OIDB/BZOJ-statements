## 题目描述

Farmer John 有 $b$ 头奶牛，有 $n$ 个农场，编号 $1 \sim n$，有 $m$ 条双向边，第 $i$ 条边连接农场 $r_i$ 和 $s_i$，该边的长度是 $l_i$。居住在农场 $p_i$ 的奶牛 A，它想送一份新年礼物给居住在农场 $q_i$ 的奶牛 B，但是奶 牛 A 必须先到 FJ（居住在编号 $1$ 的农场）那里取礼物，然后再送给奶牛 B。你的任务是：奶牛 A 至少需要走多远的路程？

## 输入格式

第一行：三个整数：$n,m,b$。

第二行到第 $m+1$ 行：每行三个整数：$r_i,s_i,l_i$，描述一条边的信息。

第 $m+2$ 行到第 $m+b+1$ 行：共 $b$ 行，每行两个整数 $p_i$ 和 $q_i$，表示住在 $p_i$ 农场的奶牛送礼物给住在 $q_i$ 农场的奶牛。

## 输出格式

共 $b$ 行，每行一个整数，表示住在 $p_i$ 农场的奶牛送礼给住在 $q_i$ 农场的奶牛至少需要走的路程。

```input1
6 7 3
1 2 3
5 4 3
3 1 1
6 1 9
3 4 2
1 4 4
3 2 2
2 4
5 1
3 6
```
```output1
6
6
10
```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \leq b \leq 2.5\times10^4$，$2 \times b \leq n \leq 5\times10^4$，$n-1 \leq m \leq 1\times10^5$，$1 \leq l_i \leq 2\times10^3$，$1 \leq p_i,q_i,r_i,s_i \leq n$。

## 题目来源

Silver