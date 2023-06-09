## 题目描述

给出两个 $n\times n$ 的矩阵，$m$ 次询问它们的积中给定子矩阵的数值和。

## 输入格式

第一行两个正整数 $n,m$。

接下来 $n$ 行，每行 $n$ 个非负整数，表示第一个矩阵。

接下来 $n$ 行，每行 $n$ 个非负整数，表示第二个矩阵。

接下来 $m$ 行，每行四个正整数 $a,b,c,d$，表示询问第一个矩阵与第二个矩阵的积中，以第 $a$ 行第 $b$ 列与第 $c$ 行第 $d$ 列为顶点的子矩阵中的元素和。

## 输出格式

对每次询问，输出一行一个整数，表示该次询问的答案。

```input1
3 2
1 9 8
3 2 0
1 8 3
9 8 4
0 5 15
1 9 6
1 1 3 3
2 3 1 2
```

```output1
661
388
```

## 数据规模与约定

对 $30\%$ 的数据，$n\le 100$。

对 $100\%$ 的数据，$n\le 2\times 10^3$，$m\le 5\times 10^4$，输入数据中矩阵元素 $<100$，$a,b,c,d\le n$。

