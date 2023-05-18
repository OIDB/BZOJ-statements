## 题目描述

有 $n$ 个城镇，每个城镇描述为平面上一个点 $(x,y)$，我们想把其中一些城镇划分在一起，以便于管理。划分在一起的城镇称之为一个区，必须保证一个区中城镇之间的距离都严格小于区中城镇到区外城镇的距离。

现在我们想知道把城镇划分成多少个区是可行的。

## 输入格式

第 $1$ 行为一个整数 $n$，表示城镇的个数。

接下来 $n$ 行，每行两个数 $x,y$，描述每个城镇的坐标。

## 输出格式

一行若干个整数，表示所有可行的城镇划分个数，数之间用一个空格隔开并且严格递增。

## 样例输入

```plain
4
-1 -1
1 1
1 -1
-1 1
```

## 样例输出

```plain
1 4
```

## 数据规模与约定

对于 $30\%$ 的数据 $1\le n\le 10$。

对于 $100\%$ 的数据 $1\le n\le 300$，$-10^4\le x,y\le 10^4$。
