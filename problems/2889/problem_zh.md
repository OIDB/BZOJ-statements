## 题目描述

给定一棵 $n$ 个点的树，求有多少种方案可以把树分为若干联通子树，且每个联通子树的大小相等。


## 输入格式

第一行一个整数 $n$。

接下来 $n-1$ 行每行两个整数 $u,v$ 表示一条 $u,v$ 之间的边。

## 输出格式

一行一个整数表示答案。

```input1
6
1 2
2 3
2 4
4 5
5 6
```

```output1
3
```

## 数据规模与约定

对于 $10\%$ 的数据，$1\leq n\leq 16$；

对于 $30\%$ 的数据，$1\leq n\leq 100$；

对于 $50\%$ 的数据，$1\leq n\leq 5\times 10^4$；

对于 $100\%$ 的数据，$1\leq n\leq 10^6$。
