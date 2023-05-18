## 题目描述

$N$ 头牛，坐标各不相同。

在 $(0,0)$ 点有个半径为 $R$ 的圆挡住了这些牛的视线，问有多少对牛是互相可见的。

## 输入格式

第一行两个整数 $N,R$。

接下来 $N$ 行，每行两个整数，表示每头牛的坐标 $(x,y)$。

## 输出格式

一行一个整数，表示能互相看到的奶牛对数。

```input1
4 5
0 10
0 -10
10 0
-10 0
```

```output1
4
```

## 样例说明 1

样例中 $4$ 头牛分别在坐标 $(0,10),(0,-10),(10,0),(-10,0)$ 的位置。圆的圆心为 $(0,0)$ 并且半径为 $5$。

$6$ 对母牛都能看到对方，除了位于圆两侧的那对母牛（位于 $(-10,0)$ 和 $(10,0)$ 的母牛不能看到对方，位于 $(0,-10) 和 $(0,10) 的母牛不能看到对方。）

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq N\leq 5\times 10^4$，$1\leq R\leq 10^6$，$-10^6\leq x,y\leq 10^6$。

## 题目来源

Gold