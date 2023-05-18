## 题目描述

在 $x$ 轴上有 $n$ 个点，每个点有 $m$ 升水。

一只虫子在坐标轴 $0$ 点上，它每个单位时间可以移动一格，每个点的水每经过 $1$ 单位时间就会消失 $1$ 升，直到全部消失。

问虫子最多可以喝到多少水，喝水的时间忽略不计。

## 输入格式

第一行两个整数 $n,m$。

第 $2$ 行到第 $n+1$ 行，每行一个点的坐标 $x_i$ 表示第 $i$ 个点的坐标。

## 输出格式

一行一个整数，表示最多可以喝到多少水。



```input1
3 15
6
-3
1
```

```output1
25
```

## 样例说明

虫子开始在 $0$ 点，它先到 $1$ 这个点喝水，再到 $-3$ ，再到 $6$。

## 数据规模与约定

对于 $100\%$ 的数据，$0 \leq n \leq 300$，$1 \leq m \leq 10^6$，$−10^4 \leq x_1, x_2,\dots,x_n \leq 10^4$。
