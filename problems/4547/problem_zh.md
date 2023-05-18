## 题目描述

有一个大小为 $n$ 的可重集 $S$，小奇每次操作可以加入一个数 $a+b$（$a,b$ 均属于 $S$），求 $k$ 次操作后它可获得的 $S$ 的和的最大值。（数据保证这个值为非负数）

## 输入格式

第一行有两个整数 $n,k$，表示初始元素数量和操作数。

第二行包含 $n$ 个整数，表示初始时可重集的元素。

## 输出格式

输出一个整数，表示和的最大值。答案对 $10^7+7$ 取模。

## 样例输入

```plain
2 2
3 6
```

## 样例输出

```plain
33
```

## 数据规模与约定

对于 $100\%$ 的数据，有 $n \le 10^5$，$k\le10^9$，$|a_i|\le10^5$。

## 题目来源

By Hzwer