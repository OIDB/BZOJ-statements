## 题目描述

每一头牛的愿望就是变成一头最受欢迎的牛。现在有 $n$ 头牛，给你 $m$ 对整数 $(a_i,b_i)$，表示牛 $a_i$ 认为牛 $b_i$ 受欢迎。这种关系是具有传递性的，如果 $u$ 认为 $v$ 受欢迎，$v$ 认为 $w$ 受欢迎，那么牛 $u$ 也认为牛 $w$ 受欢迎。你的任务是求出有多少头牛被所有的牛认为是受欢迎的。

## 输入格式

第一行两个数 $n,m$。  

接下来 $m$ 行，每行两个数 $a_i$，$b_i$，意思是 $a_i$ 认为 $b_i$ 是受欢迎的（给出的信息有可能重复，即有可能出现多个相同的 $a_i$，$b_i$）。

## 输出格式

一个数，即有多少头牛被所有的牛认为是受欢迎的。

```input1
3 3
1 2
2 1
2 3
```

```output1
1
```
## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n\leq10^4，m\leq5\times10^4$。