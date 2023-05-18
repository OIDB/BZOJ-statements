## 题目描述

一个序列的第 $1,3,5\dots$ 项被称作奇数项，第 $2,4,6\dots$ 项被称作偶数项。

一个序列 $a_{1\dots n}$ 被称作 ZigZag 序列当且仅当以下两个条件中的一个（或两个）成立：

1. 除了首项，所有的奇数项都比它的前项小且所有的偶数项都比它的前项大。
2. 除了首项，所有的奇数项都比它的前项大且所有的偶数项都比它的前项小。

一个序列 $a_{1\dots n}$ 被称作 $k$ 凹凸序列当且仅当它的最长 ZigZag 子序列（不一定是连续子序列）的长度不超过 $k$。现在有一个序列 $a_{1\dots n}$，每次可以花费 $1$ 的代价使得 $a$ 中的某一项增加或减少 $1$。我们的目的是花费最少的代价让它成为 $k$ 凹凸序列。

## 输入格式

输入的第一行包含两个正整数，分别表示数列 $a_{1\dots n}$ 的长度 $n$ 和 $k$。

接下来的 $n$ 行每行一个自然整数，依次表示数列的项。

## 输出格式

输出一个整数，表示最小代价。

## 样例输入

```plain
9 3
1
2
3
6
9
8
7
4
5
```

## 样例输出

```plain
1
```

## 样例说明

把最后一项减小 $1$，得到序列 `1 2 3 6 9 8 7 4 4`，它的最长 ZigZag 子序列之一是 `1 9 4`，长度为 $3$，符合要求。

## 数据规模与约定

前 $1$ 个测试点满足：$k=1$，$n\leq 2\times 10^4$。

第 $2\sim 8$ 个测试点满足：$k=2$，$n\leq 2\times 10^4$。

第 $9\sim 15$ 个测试点满足：$k=3$，$n\leq 2\times 10^4$。

第 $16\sim 20$ 个测试点满足：$k\leq 10$，$n\leq 10^3$。

所有测试点满足：$0\leq a_i\leq 5\times 10^4$。

## 题目来源

版权所有者：范浩强
