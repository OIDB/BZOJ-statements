## 题目描述

给出一系列点 $p_{1\cdots n}$，将其分成不多余 $m$ 个连续的段，第 $i$ 段内求一个点 $q_i$，使得 $q_i$ 到这段内点的距离的最大值的最大值最小。

## 输入格式

第一行两个整数 $n,m$。

下面 $n$ 行，每行两个整数，表示 $p_i$ 的坐标 $(x,y)$ 。

## 输出格式

第一行，$q_i$ 到这段内点的距离的最大值的最大值的最小值。

第二行，分成的段数 $k$。

下面 $k$ 行，每行两个实数，表示 $q_k$ 的坐标 $(x,y)$。

```input1
7 2
2 0
0 4
4 4
4 2
8 2
11 3
14 2
```

```output1
3.00000000
2
2.00000000 1.76393202
11.00000000 1.99998199
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq m\leq n\leq 10^5$，$|x|,|y|\leq 10^6$。