## 题目描述

神犇有一个 $n$ 个节点的图。因为神犇是神犇，所以在 $T$ 时间内一些边会出现后消失。神犇要求出每一时间段内这个图是否是二分图。这么简单的问题神犇当然会做了，于是他想考考你。

## 输入格式

输入数据的第一行是三个整数 $n,m,T$。
第 $2$ 行到第 $m+1$ 行，每行 $4$ 个整数 $u,v,start,end$。第 $i+1$ 行的四个整数表示第 $i$ 条边连接 $u,v$ 两个点，这条边在 $start$ 时刻
出现，在第 $end$ 时刻消失。

## 输出格式

输出包含 $T$ 行。在第 $i$ 行中，如果第 $i$ 时间段内这个图是二分图，那么输出“``Yes``”，否则输出“``No``”，不含引号。

```input1
3 3 3
1 2 0 2
2 3 0 3
1 3 1 2
```

```output1
Yes
No
Yes
```

## 样例说明：
$0$ 时刻，出现两条边 $1-2$ 和 $2-3$。
第 $1$ 时间段内，这个图是二分图，输出 ``Yes``。
$1$ 时刻，出现一条边 $1-3$。
第 $2$ 时间段内，这个图不是二分图，输出 ``No``。
$2$时刻，$1-2$ 和 $1-3$ 两条边消失。
第3时间段内，只有一条边 $2-3$，这个图是二分图，输出 ``Yes``。

## 数据范围

对于 $100\%$ 的数据，$n\le 100000,m\le 200000,T\le 100000$，$1\le u,v\le n$，$0\le start\le end\le T$。
