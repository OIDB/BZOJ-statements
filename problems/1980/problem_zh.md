## 题目描述

给你一个长度为 $n$ 的 $A$ 序列和一个长度为 $m$ 的 $B$ 序列，现在的任务是给 $A$ 序列的每个元素，在 $B$ 序列中找一个数跟它匹配，并且使得权值之和最小（权值为两个数的差的绝对值）。

## 输入格式

第一行输入两个正整数 $m,n$。 

接下来 $m+n$ 行，分别表示 $B,A$ 序列。

<!--原文还有一句：.........实际上似乎没这么大，
用Longint就可以保存了.......-->


## 输出格式 

输出最小的权值之和。

```input1
4 2
1
10
12
20
11
15
```

```output1
4
```

## 数据规模与约定

对于 $100\%$ 的数据，$m \le 10^6$，$n \le 2 \times 10^3$，$A_i, B_i \le 10^{30}$。