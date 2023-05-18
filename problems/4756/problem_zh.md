## 题目描述

$n$ 只奶牛构成了一个树形的公司，每个奶牛有一个能力值 $p_i$，$1$ 号奶牛为树根。

问对于每个奶牛来说，它的子树中有几个能力值比它大的。

## 输入格式

第一行一个正整数 $n$，表示有几只奶牛。

接下来 $n$ 行为 $1\cdots n$ 号奶牛的能力值 $p_i$。

接下来 $n-1$ 行为 $2\cdots n$ 号奶牛的经理（树中的父亲）。

## 输出格式

共 $n$ 行，每行输出奶牛 $i$ 的下属中有几个能力值比 $i$ 的大。

```input1
5
804289384
846930887
681692778
714636916
957747794
1
1
2
3
```

```output1
2
0
1
0
0
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n\le 10^5$。

## 题目来源

Platinum 鸣谢 Acty 提供译文。