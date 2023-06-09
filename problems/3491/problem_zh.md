## 题目描述

有一个集合 $U = \left\{ 1,2,\dots, n\right\}$, 要从中选择 $k$ 个元素作为一个子集 $A$. 若 $a \in A$, 则要求 $a * X \notin A$, 其中 $X$ 是一个给定的数.

求可选方案对 $m$ 取模后的值.

## 输入格式

第一行共四个整数,分别为题面描述中的 $n, m, k, X$

## 输出格式

共一行一个整数,为可选方案对 $m$ 取模后的值.

## 样例输入

```
6 1234 3 2
```

## 样例输出

```
9
```

## 数据范围

对于所有数据, 满足 $1 \leq n \leq 10^{18}, 2 \leq m \leq 10^6, 0 \leq k \leq 1000, 2 \leq X \leq 10$.