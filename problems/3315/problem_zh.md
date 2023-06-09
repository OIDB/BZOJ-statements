## 题目描述

一个坐标轴有 $N$ 个点，每跳到一个点会获得该点的分数，并只能朝同一个方向跳，但是每一次的跳跃的距离必须不小于前一次的跳跃距离，起始点任选，求能获得的最大分数。

## 输入格式

第一行一个整数 $N$。

接下来 $N$ 行，每行两个整数 $x_i,p_i$。

## 输出格式

一行，一个整数，表示能获得的最大分数。

```input1
6
5 6
1 1
10 5
7 6
4 8
8 10
```

```output1
25
```

## 样例说明 1

从坐标为 $4$ 的点，跳到坐标为 $5$ 的，再到坐标为 $7$ 的，再到坐标为 $10$ 的。

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq N\leq 10^3$，$1\leq x_i,p_i\leq 10^6$。

## 题目来源

Silver