## 题目描述

有一个树形结构的宾馆，$n$ 个房间，$n-1$ 条无向边，每条边的长度相同，任意两个房间可以相互到达。吉丽要给他的三个妹子各开（一个）房（间）。三个妹子住的房间要互不相同（否则要打起来了），为了让吉丽满意，你需要让三个房间两两距离相同。

有多少种方案能让吉丽满意？

## 输入格式

第一行一个数 $n$。

接下来 $n-1$ 行，每行两个数 $x,y$，表示 $x$ 和 $y$ 之间有一条边相连。

## 输出格式

让吉丽满意的方案数。

```input1
7
1 2
5 7
2 5
2 3
5 6
4 5
```
```output1
5
```

## 样例说明

方案分别为 $\{1,3,5\},\{2,4,6\},\{2,4,7\},\{2,6,7\},\{4,6,7\}$。


## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 5\times10^3$，$1 \le x\le y \le n$。

## 题目来源
By Dzy