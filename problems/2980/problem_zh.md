//时间限制：10s 空间限制：128MB
## 题目描述
$B$ 是一个正整数. 如果一个自然数 $n$ 被称为 $B$-smooth 数,那么它的质因素中没有任何一个超过 $B$。我们说和 $n$ 等价的一个 $B$-smooth 数，如果它能够表示成小于或等于 $B$ 的正整数乘积。你的任务是对给定的闭区间 $[n,n+m]$，求出他们中的 $B$-smooth 数的个数。

## 输入格式
第一行有用单个空格分隔的三个整数 $n, m$ 和 $B$。

## 输出格式
求出 $B$-smooth 数的个数.
## 样例输入
```
30 10 5
```
## 样例输出
```
4
```

## 数据规模与约定
对于 $100\%$ 的数据，$1\leq n\leq 2\times 10^9$，$1\leq m\leq 1\times 10^8$，$1\leq B\leq 1\times 10^6$。