## 题目描述

有一排 $n$ 个格子，两人轮流用 $k$ 种颜色给未染色的格子染色，要求每次染色后都不能有两个相邻的格子被染上了相同的颜色。

你需要做的是判断一个已有部分格子被染色的初始局面是先手必胜还是后手必胜。

## 输入格式

**本题有多组测试数据。**

第一行一个数 $T$，表示数据组数。

接下来每组数据的第一行两个数 $n , k$ 如题中所述，第二行 $n$ 个 $0$ 到 $k$ 的整数，$0$ 表示格子未染色，否则表示该格子的颜色，保证初始局面没有两个相邻格子同色。

## 输出格式

共 $T$ 行，每行一个字符，``y`` 表示先手必胜，``n`` 表示后手必胜。

```input1
2
5 2
0 0 1 0 0
5 1
1 0 0 0 0
```

```output1
n
y
```

## 样例说明 1

第一局游戏中局面是对称的，所以只要先手可以给格子染色，后手就可以给其对称的格子染色，故后手必胜。

第二局游戏中，先手给第 $4$ 个格子染色后，后手就不能染色了，故先手必胜。

![](https://hydro.org.cn/d/bzoj/p/2410/file/pic1.jpg)

## 数据规模与约定

对于 $100\%$ 的数据，保证 $1\le T \le 20 , 1\le k \le n\le 10^5$ 。