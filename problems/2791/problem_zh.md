## 题目描述

给定一个 $n$ 个顶点的有向图，每个顶点有且仅有一条出边。

对于顶点 $i$，记它的出边为 $(i,a_i)$。

再给出 $q$ 组询问，每组询问由两个顶点 $a,b$ 组成，要求输出满足下面条件的 $x,y$：

1. 从顶点 $a$ 沿着出边走 $x$ 步和从顶点 $b$ 沿着出边走 $y$ 步后到达的顶点相同。
2. 在满足条件 $1$ 的情况下 $\max(x,y)$ 最小。
3. 在满足条件 $1$ 和 $2$ 的情况下 $\min(x,y)$ 最小。
4. 在满足条件 $1,2$ 和 $3$ 的情况下 $x\ge y$。

如果不存在满足条件 $1$ 的 $x,y$，输出 `-1 -1`。

## 输入格式

第一行两个正整数 $n,q$。  
第二行 $n$ 个正整数 $a_{1\dots n}$。  
接下来 $q$ 行，每行两个数 $a,b$ 表示一组询问。

## 输出格式

共 $q$ 行，每行表示一个询问的答案。

```input1
12 5
4 3 5 5 1 1 12 12 9 9 7 1
7 2
8 11
1 2
9 10
10 5
```

```output1
2 3
1 2
2 2
0 1
-1 -1
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n,q\leq 5\times 10^5$，$1\leq a,b,a_i\leq n$。