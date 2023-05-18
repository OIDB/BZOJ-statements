## 题目描述

给你一个由'``B``'和'``W``'组成的序列，将其按分成最多的区间且每个区间的'``B``':'``W``'的值相等。

## 输入格式

多组数据，第一行一个整数 $T$ 表示数据组数。

每组数据的第一行为一个整数 $n$，接下来 $n$ 行，每行一个整数 $k$ 和一个字符（'``B``'或'``W``'）表示在上一个序列后有一个长度为 $k$ 的'``B``'或'``W``'的序列。

## 输出格式

共 $T$ 行，每行一个整数表示能分成的最多的区间数。

```input1
3
3
1 B
3 W
2 B
4
3 W
3 B
9 W
1 B
2
2 W
3 W
```

```output1
2
3
5
```

## 数据范围

对于 $100\%$ 的数据，序列的总长度不超过 $10^9$。