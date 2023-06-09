## 题目描述

有一棵 $n$ 个节点的树，树上的每个节点有一个小写字母。

定义一个 **树上子串** 为从某个节点向子节点移动若干步，把路径上的字母拼起来得到的字符串。

现在你需要求出有多少个本质不同的 **树上子串** 以及回答 $q$ 次形如「在所有本质不同的树上子串中，字典序第 $k-1$ 小的 **树上子串** 是什么」的询问。


## 输入格式

第一行两个整数 $n,q$。

第二行 $n$ 个小写字母，第 $i$ 个字母表示结点 $i$ 上的字母。

接下来 $n-1$ 行，每行两个点 $u,v$ 表示树上一条 $u,v$ 之间的边。

接下来 $q$ 行，每行一个整数 $k$ 表示一个询问。

## 输出格式

第一行一个整数表示本质不同的树上子串个数。

接下来 $q$ 行，每行依次表示一个询问的答案。

特殊的，若 $k=1$ 请直接输出一个空行；否则若不存在字典序为 $k-1$ 的子串，输出一行一个 `-1`。

```input1
8 1
abcbbaca
1 2
2 3
1 4
4 5
4 6
4 7
1 8 
5
```

```output1
12
aba
```

## 数据规模与约定

对于 $12\%$ 的数据，$1\leq n\leq 10$；

对于另外 $48\%$ 的数据，树的形态是一条链；

对于 $100\%$ 的数据，$1\leq n\leq 2.5\times 10^5$，$1\leq q\leq 5\times 10^4$。

