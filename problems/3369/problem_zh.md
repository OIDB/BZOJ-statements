## 题目描述

奶牛们只学过加和减．她们写下了含有 $N$ 项的表达式，比如：

$$
1+4-2-1+10-6
$$

贝茜认识到地加上不同的括号，表达式就会有不同的值。请帮她计算出表达式的最大值。

## 输入格式

第 $1$ 行：整数 $N$；

第 $2$ 到 $N+1$ 行：每行是一个整数 $K$，表示表达式中的一项。正整数 $K$ 表示 $+K$，负整数 $K$ 表示 $-K$。

## 输出格式

一个整数，通过适当地加括号使表达示得到的最大值．

```input1
6
1
4
-2
-1
10
-6
```

```output1
20
```

## 样例解释

$$
1+4 -(2- (1+ 10) -6)=20
$$

## 数据范围与约定

对于 $100\%$ 的数据，$1 ≤ N ≤ 10$，$-100 ≤ K ≤ 100$。

## 题目来源

Orange


