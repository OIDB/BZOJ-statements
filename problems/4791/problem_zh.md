## 题目描述

俄罗斯套娃是一些尺寸递增的木制雕像，它们可以嵌套在一起。每个套娃可以放进一个更大的套娃，也可以被放入一个更小的套娃。每个套娃内部最多只能直接嵌套一个套娃，但是那个套娃内部还可以继续嵌套。

给定 $n$ 个尺寸互不相同的套娃，按尺寸从小到大依次编号为 $1$ 到 $n$ 。如果套娃 $a$ 被直接嵌入套娃 $b$，那么我们称 $b$ 是 $a$ 的父亲，如果一个套娃没有父亲，那么我们称它是自由的。一组镶嵌方案可以用每个套娃的父亲来表示。

我们可以每步可以做以下两种操作中的任意一种：

1. 把一个自由的套娃直接嵌入一个更大的没有被放入东西的套娃。

2. 选择一个不自由的套娃，将其从其父亲中取出。

给定初始局面，请计算达到目标局面的最小的操作步数。

## 输入格式

第一行包含一个正整数 $n$，表示套娃的个数。  
第二行包含 $n$ 个整数 $p_1,p_2,\cdots,p_n$，依次表示初始局面中每个套娃的父亲，$0$ 表示自由套娃。  
第三行包含 $n$ 个整数 $q_1,q_2,\cdots,q_n$，依次表示目标局面中每个套娃的父亲，$0$ 表示自由套娃。  
输入数据保证初始局面和目标局面均合法。

## 输出格式

输出一行一个整数，即最小操作步数。



```input1
7
3 5 4 0 7 0 0
3 5 0 6 7 0 0
```




```output1
2
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n\le 10^5$，$0\le p_i,q_i\le n$。