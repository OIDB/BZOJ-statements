## 题目描述

小 N 最近在做关于树的题。今天她想了这样一道题，给定一棵 $n$ 个节点的树，节点按 $1\sim n$ 编号，一开始每个节点上的权值都是 $0$，接下来有 $m$ 个操作。第一种操作是修改，给出 $4$ 个整数 $x,y,a,b$，对于 $x$ 到 $y$ 路径上加上一个首项是 $a$，公差是 $b$ 的等差数列，因为小 N 十分谨慎，所以她每做完一个修改操作就会保存一次，初始状态是第 $0$ 次保存的局面。第二种操作是求和，给出 $2$ 个整数 $x,y$，输出 $x$ 到 $y$ 路径上所有节点的权值和。第三种操作是读取之前第 $x$ 次保存的局面，所有节点的状态回到之前第 $x$ 次保存的状态。现在请你对每一个求和操作输出答案。

## 输入格式

第一行两个整数 $n,m$ 表示节点个数和操作次数。

接下来 $n-1$ 行每行 $2$ 个整数 $u_i,v_i$ 表示了这棵树中 $u_i$ 和 $v_i$ 这 $2$ 个节点间有边相连。

接下来 $m$ 行每行先有一个字符表示了操作的类型；同时为了保证在线，我们设 $t$ 表示上一次输出的答案：
* 如果是 `c`，那么代表了一个修改操作，接下来有 $4$ 个整数 $x1,y1,a,b$，为了使得询问在线，正确的 $x=x1\text{ xor }t$，$y=y1\text{ xor }t$，如果之前没有输出过那么当成 $0$。
* 如果是 `q`，那么代表了一个求和操作，接下来有两个整数 $x1,y1$，和修改操作一样需要  $\text{xor }t$。
* 如果是 `l`，那么代表了一次读取操作，接下来一个整数 $x1$，正确的 $x=x1\text{ xor }t$。

## 输出格式

对于每一个求和操作，输出求和后的值。

```input1
5 7
1 2
2 3
3 4
4 5
c 2 5 2 3
c 3 4 5 10
q 1 3
l 13
q 13 15
l 6
q 6 4
```

```output1
12
7
7
```

## 数据规模与约定

* $100\%$ 的数据中 $n,m \leq 10^5$，$0 \leq a,b \leq 1000$，$0 \leq x1,y1 \leq 10^1$，修改次数 $<\frac{m}{2}$，不会读取没保存的局面。

## 题目来源

持久化线段树