## 题目描述

对于一个长度为 $n$ 的序列 $a_1,a_2,\cdots,a_n$ ，其前缀和 (Prefix Sum) $S_i$ 为前 $i$ 个元素的和，即 $\sum_{k=1}^i a_i$。而前缀和的前缀和 (Preprefix Sum) 就是把前缀和序列 $S_1,S_2,\cdots,S_n$ 作为原序列，再求一次前缀和。记再次求得的前缀和序列的第 $i$ 位为 $SS_i$ 。

现在给定一个长度为 $n$ 的序列 $a_1,a_2,\cdots,a_n$ ，有两种操作:

1. `Modify i x` 将 $a_i$ 的值改为 $x$ 。
2. `Query i` 询问$SS_i$的值。

请编写一个程序来实现这两种操作。

## 输入格式

第一行给出两个整数 $n,m$ 。分别表示序列长度和操作个数
接下来一行有 $n$ 个数，即给定的序列 $a_1,a_2,\cdots,a_n$
接下来 $m$ 行，每行对应一个操作，格式见题目描述

## 输出格式

对于每个询问操作，输出一行，表示所询问的 $SS_i$ 的值。

## 样例输入

```plain
5 3
1 2 3 4 5
Query 5
Modify 3 2
Query 5
```

## 样例输出

```plain
35
32
```

## 数据规模与约定

$1\le n,m\le 10^5$，且在任意时刻$1\le a_i\le 10^5$

## 题目来源

Katharon+#1
