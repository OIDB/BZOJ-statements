## 题目描述

小白非常喜欢跑步，所以他经常在校园内跑步（其实是想看美女~）。校园可以看成由 $n$ 个地区，由 $m$ 个道路连接。我们小白早上从一个地点出发，但是不知道怎么跑才好。小白有个习惯，不会沿着刚刚经过的道路再返回（比如从 $a$ 到 $b$ 经过 $c$ 道路，下一次，不会再沿着 $c$ 从 $b$ 返回 $a$）。

小白想知道从他出发的地点，经过 $Q$ 条路，到达每个点的方案数。这样方便他去选择。

## 输入格式

第一行四个整数 $n,m,s,Q$。表示有 $n$ 个地区，$m$ 条道路，从 $s$ 出发，需要经过 $Q$ 条路。

下面 $m$ 行，每行两个整数表示 $a,b$ 之间有条道路。

## 输出格式

一共 $n$ 行，每行一个整数表示从 $s$ 到 $i$ 的方案数。（$\bmod 45989$）

```input1
10 20 9 10
1 5
5 10
10 4
10 2
10 7
4 3
10 9
2 8
5 6
6 1
2 10
4 7
9 10
9 6
7 3
7 3
7 2
1 8
9 7
4 5
```

```output1
17420
41928
35701
40814
31937
22933
5754
15848
43620
10819
```

## 数据规模与提示

对于 $100\%$ 的数据，$n \le 30$，$m \le 60$，$Q \le 10^{16}$。
