## 题目描述

有 $n$ 个点（编号 $1$ 到 $n$）组成的无向图，已经为你连了 $m$ 条边。请你再连 $k$ 条边，使得所有的点的度数都是偶数。求有多少种连的方法。

要求你连的 $k$ 条边中不能有重边，但和已经连好的边可以重。不允许自环的存在。求连边的方法数。我们只关心它模 $10007$ 的余数。

## 输入格式

输入的第一行有三个自然数，分别表示点数 $n$，已经连好的边数 $m$，和你要连的边数 $k$。保证 $k\leq \frac{n(n-1)}2$。

接下来 $m$行每行两个整数 $x,y$，描述了一条连接 $x$ 和 $y$ 的边。

## 输出格式

输出一个整数，表示连边的方法数模 $10007$ 的余数。

## 样例输入

```plain
5 1 4
1 2
```

## 样例输出

```plain
13
```

## 样例说明

以下是 $13$ 种连边的方法（只显示你连的边）：

```plain
{(1,2),(1,3),(1,4),(3,4)}
{(1,2),(1,3),(1,5),(3,5)}
{(1,2),(1,4),(1,5),(4,5)}
{(1,2),(2,3),(2,4),(3,4)}
{(1,2),(2,3),(2,5),(3,5)}
{(1,2),(2,4),(2,5),(4,5)}
{(1,2),(3,4),(3,5),(4,5)}
{(1,3),(2,4),(3,5),(4,5)}
{(1,3),(2,5),(3,4),(4,5)}
{(1,4),(2,3),(3,5),(4,5)}
{(1,4),(2,5),(3,4),(3,5)}
{(1,5),(2,3),(3,4),(4,5)}
{(1,5),(2,4),(3,4),(3,5)}
```

## 数据规模与约定

$30\%$ 的数据满足：$n\leq 200$。

$100\%$ 的数据满足：$n\leq 10^3$，$m\leq n,k\leq \min(10^3,\frac{n(n-1)}2)$。

（修着按：在修缮本题时，发现了在题目末尾的另一段数据范围，经测试，该数据范围与数据不符，现将其附于下方：

对于 $20\%$ 的数据，$4\leq n\leq 100$。

对于 $40\%$ 的数据，$4\leq n\leq 5\times 10^3$。

对于 $100\%$ 的数据，$4\leq n\leq 5\times 10^4$，$1\leq m\leq 10$，$m\leq n$，所有出现的整数均不超过 $32$ 位含符号整数。 ）

## 题目来源

版权所有者：范浩强
