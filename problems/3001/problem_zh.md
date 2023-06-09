## 题目描述

在一个神秘的岛上，有许许多多水井，水井只有两种，圆井和方井，两种井各有 $ n $ 个，水井两两相通。

如果两个水井形状相同，则水井下通道的流向是不确定的。可以任意修改。

如果两个水井形状不同，则水井下通道的流向是确定的。若两个水井间的距离 $ D_{ij}>d $，则圆井流向方井，否则方井流向圆井。

这里的 $ D_{ij} $ 指的是曼哈顿距离（ $ |x_i-x_j|+|y_i-y_j| $ )， $ d $ 为给定值。

如果某三个井 $ i,j,k $ ,它们形状不完全相同，且它们之间的连的边是  $ i \to j,j \to k,k \to i $。那么就会出现一次灵异现象。

现在要问的是，通过改变同形状水井通道的流向，使得灵异现象出现的最多次和最少次。

## 输入格式

第一行两个正整数 $ n,d $。

接下来 $ n $ 行 $ x_i,y_i $ 描述第 $ i $ 个圆井的坐标。

再接下来 $ n $ 行 $ x_j,y_j $ 描述第 $ j $ 个方井的坐标。

## 输出格式

两个数依次为灵异现象出现最少的次数，最多的次数，中间用一个空格隔开。

## 样例输入

```
2 1
1 2
1 1
3 1
2 2
```

## 样例输出

```
0 2
```

## 数据规模与约定

对于 $100\%$ 的数据， $ n \leq 1\times 10^5 $， $ 1 \leq x,y,d \leq 1\times 10^5 $ 且为整数。
