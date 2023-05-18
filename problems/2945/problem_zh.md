## 题目描述

在一个气垫船厂用不同高度方块建造了一个测试轨道。一条完美的轨道，被称做 lollobrigida，是相邻两个方块的高度不同且连续的三个方块的高度既不是递减也不是递增的轨道。

用更形式的表达，设 $h_1,h_2,\cdots,h_n$ 是建造轨道的方块的高度。如果任意 $1\le i\le n-2$ 都有满足下面条件之一：

- $h_i<h_{i+1}$ 且 $h_{i+1}>h_{i+2}$；
- $h_i>h_{i+1}$ 且 $h_{i+1}<h_{i+2}$。

这样我们便称一条轨道为 lollobrigida。

**例子**：

我们不可能用下面一组高度的方块来建造 lollobrigida：$3,3,3,5,2$，因为两个高度为 $3$ 的方块会相邻或者会出现下列情况：$(2,3,5)$ 或者 $(5,3,2)$，这些都是不允许的。

这儿有一个用另一组高度的方块建造的 lollobrigida 的例子 $(3,2,5,2,3,1)$。我们也可以用这些方块建造其他不同的 lollobrigidas。

你需要编写一个程序，检查是否能建造 lollobrigida。

## 输入格式

第一行有一个正整数 $d$ 表示输入数据的组数。接下来的一行是第一组数据。

在每组数据的第一行有一个正整数 $n$，表示方块的个数。

接下来的 $n$ 行中每行有一个正整数 $h$ 表示一个方块的高度。

## 输出格式

应该有 $d$ 行，一个表示一组数据。每一行都有一个单词，第 $i$ 行的单词：

- `TAK`（波兰语中是的意思），如果第 $i$ 组数据可以建造 lollobrigida；
- `NIE`（波兰语中否的意思），不可以建造。

```input1
2
5
3
3
3
52
6
3
3
1
5
2
2
```
```output1
NIE
TAK
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le d\le 100$，$3\le n\le 10^6$，$1\le h\le 10^9$。
