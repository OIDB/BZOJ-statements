## 题目描述

如果一个字符串 $S$ 是 $k$（$k\ge 1$）个相同字符串 $T$ 拼接而成（不能重叠），$|T|=l≥1$，那么称 $S$ 是一个 $(k,l)$ 重复串，例如串 $S=\text{abaabaabaaba}$ 就是一个 $(4,3)$ 重复串，其中 $T=\text{aba}$。

给定一个字符串 $U$，$U_i\in\{\text{a},\text{b}\}$。求 $U$ 的所有是重复串的子串中最大的 $k$ 值。

输入保证答案不超过 $4$。


## 输入格式

第一行一个整数 $n$,表示 $U$ 的长度。

下面 $n$ 行，每行顺次给出一个串中的字符。

## 输出格式

一个整数 $k$。



```input1
17
b
a
b
b
a
b
a
a
b
a
a
b
a
a
b
a
b
```



```output1
4
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n\leq 5\times 10^4$。
