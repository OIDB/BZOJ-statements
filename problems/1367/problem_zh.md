## 题目描述

给定一个长度为 $n$ 的序列 $t$，求一个长度为 $n$ 的递增序列 $z$ 满足 $R=\sum_{i=1}^n|z_i-t_i|$ 最小，求这个最小值。

## 输入格式

第一行一个整数 $n$ 表示序列长度。

接下来 $n$ 行每行一个整数 $t_i$。

## 输出格式

一个整数 $R$。



```input1
7
9
4
8
20
14
15
18
```



```output1
13
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n\leq 10^6$，$0\leq t_k\leq 2\times 10^9$。
