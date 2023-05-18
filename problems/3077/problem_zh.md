## 题目描述

一个集合 $\{1,2,3,\cdots,2\times k-1\}$，选出其中所有大小为 $k-1$ 的子集。视所有集合为点，若两个集合之间没有公共元素，则在两个集合之间连一条边，边权为 $1$。图上两个点之间的距离定义为两个点之间的最长路长度。图的最长距离定义为所有点对中距离最大的点对的距离。给定 $k$，询问图的最长距离以及有多少对点的距离等于图的最长距离。特别的：$(1,2),(2,1)$ 算两对点。

## 输入格式

多组数据。第一行一个整数，数据组数 $T$。

接下来 $T$ 行，每行一个正整数 $k$。

## 输出格式

每组数据输出一行两个整数表示答案。由于答案可能很大所以请输出 $\bmod (10^9+7)$ 后的值。

```input1
1
3
```

```output1
2 60
```

## 数据规模与约定

对于 $100\%$ 的数据，$2\le n\le 10^5$，$T\le 25$。
