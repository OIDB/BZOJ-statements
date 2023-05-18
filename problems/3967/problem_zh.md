## 题目描述

一个最基本的算数法则就是大于 $1$ 的整数都能用 $1$ 个或多个素数相乘的形式表示出来。当然，可以安排出多种的质因子排列方案，例如：$10=2\times 5=5\times 2,20=5\times 2\times 2=2\times 5\times 2=2\times 2\times 5$。

让我们用 $f(k)$ 表示 $k$ 的质因子排列方案数，如 $f(10)=2$，$f(20)=3$。

给你一个正整数 $n$，至少有一个 $k$ 使得 $f(k)=n$，我们想知道最小的 $k$ 是多少。

## 输入格式

输入文件至多有 $1000$ 组数据，

每组数据单独成行，包含一个正整数 $n$。

## 输出格式

对于每组数据，输出他的问题 $n$ 和最小的满足 $f(k)=n$ 的 $k$。

```input1
1
2
3
105
```

```output1
1 2
2 6
3 12
105 720
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n,k\leq 2^{63}-1$。
