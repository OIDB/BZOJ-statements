## 题目描述

给定一个数 $n$，有一个数 $x$，每次你可以猜在 $[1,n]$ 中的数，假设是 $y$，如果 $x = y$，游戏结束，如果没猜中，则告诉你 $\gcd(x,y)$，然后继续猜，直到猜中为止。  
现在问给定 $n$ 的情况下，最坏情况下最少要多少次猜中。

## 输入格式

共一行，一个整数 $n$。 

## 输出格式

最坏情况下最少猜中次数。

```input1
6
```



```output1
2
```

## 数据规模与约定

对于 $100\%$ 的数据，$2 \leq n \leq 10000$，$1 \leq x \leq n$。  


## 来源

neerc2011