## 题目描述

老 C 是个程序员。

作为一个优秀的程序员，老 C 拥有一个别具一格的键盘，据说这样可以大幅提升写程序的速度，还能让写出来的程序在某种神奇力量的驱使之下跑得非常快。

小 Q 也是一个程序员。有一天他悄悄潜入了老 C 的家中，想要看看这个键盘究竟有何妙处。他发现，这个键盘共有 $n$ 个按键，这 $n$ 个按键虽然整齐的排成一列，但是每个键的高度却互不相同。聪明的小 Q 马上将每个键的高度用 $1 - n$ 的整数表示了出来，得到一个 $1 - n$ 的排列$h_1,h_2,...,h_n$。

为了回去之后可以仿造一个新键盘（新键盘每个键的高度也是一个 $1- n$ 的排列），又不要和老 C 的键盘完全一样，小 Q 决定记录下若干对按键的高度关系。作为一个程序员，小 Q 当然不会随便选几对就记下来，而是选了非常有规律的一些按键对：对于 $i=2,3,...,n$，小 Q 都记录下了一个字符 `<` 或者 `>`，表示 $h_{\frac i 2}<h_i$ 或者$h_{\frac i 2}>h_i$。于是，小 Q 得到了一个长度为 $n-1$ 的字符串，开开心心的回家了。

现在，小 Q 想知道满足他所记录的高度关系的键盘有多少个。虽然小 Q 不希望自己的键盘和老 C 的完全相同，但是完全相同也算一个满足要求的键盘。答案可能很大，你只需要告诉小 Q 答案 $\bmod 1000000007$ 之后的结果即可。

## 输入格式

输入共一行，包含一个正整数 $n$ 和一个长度为 $n-1$ 的只包含 `< `和 `> `的字符串，分别表示键盘上按键的数量，和小 Q 记录的信息，整数和字符串之间有一个空格间隔。

## 输出格式

输出共一行，包含一个整数，表示答案 $\bmod 1000000007$ 后的结果。

## 样例输入 #1

```
5 <>><
```

## 样例输出 #1

```plain
3
```

## 样例输入 #2

```plain
5 <<<<
```

## 样例输出 #2

```plain
8
```

## 样例输入 #3

```plain
5 <<>>

```

## 样例输出 #3

```plain
18
```

## 样例解释

【输入输出样例 1 说明】 共 $5$ 个按键，第 $1$ 个按键比第 $2$ 个按键矮，第 $1$ 个按键比第 $3$ 个按键高，第 $2$ 个按键比第 $4$ 个

按键高，第 $2$ 个按键比第 $5$ 个按键矮。

这 $5$ 个按键的高度排列可以是 $(2,4,1,3,5) , (3,4,1,2,5) , (3,4,2,1,5) $。

【输入输出样例 2 说明】

这 $5$ 个按键的高度排列可为 $(1,2,3,4,5) , (1,2,3,5,4) , (1,2,4,3,5) , (1,2,4,5,3) , (1,2,5,3,4) ,(1,2,5,4,3) , (1,3,2,4,5) , (1,3,2,5,4) $。

## 数据范围与约定

![](https://cdn.luogu.com.cn/upload/pic/5095.png)


