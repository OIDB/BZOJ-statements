## 题目描述

废话不多说，反正小 w 要发喜糖啦！！ 小 w 一共买了 $n$ 块喜糖，发给了 $n$ 个人，每个喜糖有一个种类。这时，小 w 突发奇想，如果这 $n$ 个人相互交换手中的糖，那会有多少种方案使得每个人手中的糖的种类都与原来不同。 两个方案不同当且仅当，存在一个人，他手中的糖的种类在两个方案中不一样。

## 输入格式

第一行，一个整数 $n$ 接下来 $n$ 行，每行一个整数，第 $i$ 个整数 $A_i$ 表示开始时第 $i$ 个人手中的糖的种类。

## 输出格式

一行一个整数 $Ans$，表示方案数模 $10^9+9$ 的结果。

```input1
6
1
1
2
2
3
3
```

```output1
10
```

## 数据规模与约定

对于 $100\%$ 的数据，满足 $1\leq A_i\leq k$，$k\leq n$，$n\leq 2000$。