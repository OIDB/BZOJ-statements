## 题目描述

有一张 $n\times m$ 的网格，初始位置 $(i,j)$ 上的值是给定的 $a_{i,j}$，网格上有一个位于 $(x,y)$ 的基础点。

需要你维护这个网格，支持 $q$ 次如下操作之一：

- `0 x1 y1 x2 y2`，询问以 $(x,y)$ 为基础，向上扩展 $x_1$ 行，向下扩展 $x_2$ 行，向左扩展 $y_1$​ 列，向右扩展 $y_2$ 列得到的矩阵里所有数字的最大公约数；
- `1 x1 y1 x2 y2 c`，对以 $(x_1,y_1)$​​ 为左上角，$(x_2,y_2)$ 为右下角的矩阵中的每个位置都加上 $c$​​。

## 输入格式

第一行两个正整数 $n,m$ 表示网格大小。

第二行两个正整数 $x,y$​ 表示基础点的坐标。

第三行一个整数 $q$ 表示操作次数。

接下来一个 $n$ 行 $m$ 列的矩阵表示初始每个位置上的值。

接下来 $q$ 行，每行一个操作，操作格式见题目描述。

## 输出格式

对于每次询问操作，输出一行一个整数表示答案。

```input1
2 2
1 1
4
6 12
18 24
0 0 0 1 0
1 1 1 1 2 6
1 2 1 2 2 6
0 0 0 1 1
```

```output1
6
6
```

## 数据规模与约定

对于 $20\%$ 的数据，$1\leq n,m\leq 100$，$1\leq q\leq 2\times 10^4$；

对于另外 $40\%$ 的数据，$n=1,1\leq m\leq 5\times 10^5$，$1\leq q\leq 10^5$。

对于剩余 $40\%$ 的数据，$1\leq n\times m\leq 5\times 10^5$，$1\leq q\leq 10^5$。

对于 $100\%$​​​ 的数据，$a_{i,j}$​​ 始终是不超过 $2^{62}-1$​​ 的正整数，且在每种数据中均有一半的数据满足所有 **修改** 都有 $x_1=x_2,y_1=y_2$。

