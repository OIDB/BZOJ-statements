## 题目描述

某人在山上种了 $n$ 棵小树苗。冬天来了，温度急速下降，小树苗脆弱得不堪一击，于是树主人想用一些塑料薄膜把这些小树遮盖起来，经过一番长久的思考，他决定用 $3$ 个 $l\times l$ 的正方形塑料薄膜将小树遮起来。我们不妨将
山建立一个平面直角坐标系，设第 $i$ 棵小树的坐标为 $(x_i,y_i)$，$3$ 个 $l\times l$ 的正方形的边要求平行与坐标轴，一个点如果在正方形的边界上，也算作被覆盖。当然，我们希望塑料薄膜面积越小越好，即求 $l$ 的最小值。

## 输入格式

第一行有一个正整数 $n$，表示有多少棵树。  
接下来有 $n$ 行，第 $i+1$ 行有两个整数 $x_i$，$y_i$，表示第 $i$ 棵树的坐标，保证不会有两个树的坐标相同。

## 输出格式

一行，输出最小的 $l$ 值。

```input1
4
0 1
0 -1
1 0
-1 0
```

```output1
1
```

## 数据规模与约定

对于 $100\%$ 的数据，有 $n\leq2\times10^4$。