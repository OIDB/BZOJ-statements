

## 题目描述

你有一个 $n \times m$ 的矩形，一开始所有格子都是白色，然后给出一个目标状态的矩形，有的地方是白色，有的地方是黑色，你每次可以选择一个连通块（四连通块，且不要求颜色一样）进行染色操作（染成白色或者黑色）。问最少操作次数。

## 输入格式

第一行两个数 $n$，$m$ 表示矩形大小。  
接下来 $n$ 行描述目标状态，每行 $m$ 个字符，`W​` 表示白色，`B` 表示黑色。

## 输出格式

一行一个整数表示操作数。

```input1
3 3
WBW
BWB
WBW

```

```output1
2
```

## 数据规模和约定

对于 $100\%$ 的数据 $n \leq 50，m \leq 50$。    
对于 $15\%$ 的数据 $n \times m \leq 15$。     
另外 $15\%$ 的数据 $m = 1$。   