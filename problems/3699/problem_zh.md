## 题目描述

GAL 喜欢自娱自乐，这次她拿出了 $3\times N$ 的非负整数，分配到 $3$ 个长度为 $N$ 的数组 $A,B,C$ 中。她对这个数组的元素进行各种各样的运算，探究各种各样的问题，乐在其中。

现在她定义三个数组的 $GAL$ 值，$GAL(A,B,C)=\sum\limits_{i=1}^n(A[i]-B[i])\times C[i]$。她要你求出 $GAL(A,B,C)$ 的最大值。

## 输入格式

第一行包含两个数 $T$ 和 $N$，$T$ 是数据组数。
接下来 $T$ 行，每行包含 $3\times N$ 个数。

## 输出格式

输出包含T行，每行输出最大的 $GAL(A,B,C)$。

```input1
1 2
4 1 8 2 0 5
```

```output1
46
```

## 数据规模与约定

$1\le n\le 25$
