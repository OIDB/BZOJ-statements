## 题面描述

$n$ 个点 $m$ 条边的无向图被分成 $k$ 个部分。每个部分包含一些点。

请选择一些关键点，使得每个部分恰有一个关键点，且每条边至少有一个端点是关键点。

## 输入格式

第一行三个整数 $n$,$m$,$k$.

接下来 $m$ 行，每行两个整数 $a,b$, 表示有一条 $a,b$ 间的边。

接下来 $k$ 行，每行第一个整数为 $w$，表示这个部分有 $w$ 个点；接下来 $w$ 个整数，为在这个部分中的点的编号。

## 输出格式

若可能则输出 `TAK`, 否则输出 `NIE`

## 样例输入

```
6 5 2
1 2
3 1
1 4
5 2
6 2
3 3 4 2
3 1 6 5
```

## 样例输出
```
TAK
```

## 数据范围

对于全部的测试点,保证 $1 \leq k, w \leq n \leq 10^6, \sum w = n, 1 \leq a,b \leq n, 0 \leq m \leq 10^6$.