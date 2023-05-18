## 题目描述

第二关和很出名的斐波那契数列有关，地球上的 OIer 都知道：$F_1=1, F_2=2, F_i=F_{i-1}+F_{i-2}$，每一项都可以称为斐波那契数。现在给一个正整数 $N$，它可以写成一些斐波那契数的和的形式。如果我们要求不同的方案中不能有相同的斐波那契数，那么对一个 $N$ 最多可以写出多少种方案呢？

## 输入格式

只有一个整数 $N$。

## 输出格式

一个方案数

## 样例输入

```plain
16
```

## 样例输出

```plain
4
```

## 样例解释

$16=3+13=3+5+8=1+2+13=1+2+5+8$.

## 数据规模与约定

对于 $30\%$ 的数据，$n\le 256$。
对于 $100\%$ 的数据，$n\le 10^{18}$。
