## 题目描述

给定平面上的 $n$ 个点，其中有一些是红的，其他是蓝的。现在让你找两条平行的直线，使得在保证不存在一个蓝色的点被夹在两条平行线之间，不经过任何一个点，不管是蓝色点还是红色点的前提下，被夹在平行线之间的红色点个数最多是多少？

## 输入格式

第 $1$ 行一个整数 $n$。

第 $2$ 到 $n+1$ 行，每行是一个点的坐标以及它的颜色。坐标用 $2$ 个绝对值 $<10^9$ 的整数表示颜色用 `R` 或 `B` 表示。

## 输出格式

第 $1$ 行仅一个整数，被夹在平行线之间的红色点个数的最大值。

```input1
4
0 0 R
0 1 B
1 1 R
1 0 B
```

```output1
2
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n\le 10^3$。