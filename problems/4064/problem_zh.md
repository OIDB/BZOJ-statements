

## 题目描述
 与当地鞋匠协会发生冲突的瓦维尔城堡的龙决定将它的狩猎场移出克拉科夫以减少敌对的邻居数量。

现在他正在给和平而宁静的 Bytes 王国带来灾难与恐怖。

在 Bytes 王国有 $n$ 条河流，每一条河流都是一条直线（你可以认为 Bytes 王国就像是欧几里得平面上被一些直线划分的一些区域），不存在三条河流共用同一个点，河流们将王国划分成了一些区域。

幸运的是，现在王国里有 $m$ 个勇士。每个勇士都发誓要保护其所在的区域。王国也许就因此受到了长远持久的保护？

我们所知道的只有龙不会攻击存在至少一个勇士的区域。

勇士们因为他们的勇气被人所熟知，然而他们的智力却低的可怕，他们不会离开自己所在的区域，只会保护所在的区域。

给出一个王国的地图，和勇士的坐标，请你计算是否所有的区域都被保护到了。
## 输入格式
第一行一个正整数 $T$，表示有 $T$ 组数据。

每组数据第一行两个正整数 $n$ 和 $m$，表示有 $n$ 条河流，$m$ 个勇士。

接下来 $n$ 行，第 $j$ 行三个整数 $A_j, B_j, C_j$，表示第 $j$ 个河流的直线方程是 $A_j * x + B_j * y + C_j = 0$，三个数字的绝对值都不超过 $10000$。

接下来 $m$ 行，第 $i$ 行两个整数 $X_i, Y_i$，表示第 $i$ 个勇士的坐标是 $(X_i, Y_i)$，$-10^9 <= X_i, Y_i <= 10^9$。

你可以认为没有一个勇士站在河流上（如果他这么做他的铠甲会很快生锈呢）。两个勇士的坐标可能相同。

不存在两条河流是重合的直线，不存在三条河流共用同一个点。
## 输出格式
对于每组数据输出一行，如果每个区域都可以被保护，输出 `PROTECTED`，否则输出`VULNERABLE`。

```input1
2
3 7
0 1 0
1 0 0
1 1 -3
1 1
5 -1
3 2
2 -2
-2 6
-1 -2
-8 4
1 1
0 1 0
0 1

```

```output1
PROTECTED
VULNERABLE
```

## 数据规模与约定

对于 $100\%$ 的数据满足，$1 \le n\le 100$，$1\le m \le 5\times 10^4$，$-10^9 \le X_i,Y_i\le 10^9$。


