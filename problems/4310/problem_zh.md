## 题目描述

很久很久以前，森林里住着一群跳蚤。一天，跳蚤国王得到了一个神秘的字符串，它想进行研究。

首先，他会把串分成不超过 $k$ 个子串，然后对于每个子串 $S$，他会从 $S$ 的所有子串中选择字典序最大的那一个，并在选出来的 $k$ 个子串中选择字典序最大的那一个。他称其为“魔力串”。

现在他想找一个最优的分法让“魔力串”字典序最小。

## 输入格式

第一行一个整数 $k$。

## 输出格式

输出一行，表示字典序最小的“魔力串”。

```input1
13
bcbcbacbbbbbabbacbcbacbbababaabbbaabacacbbbccaccbcaabcacbacbcabaacbccbbcbcbacccbcccbbcaacabacaaaaaba
```

```output1
cbc
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq k\leq |S|\leq 10^5$。