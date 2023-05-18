## 题目描述

给定一棵树 $T=(V,E)$，其中 $V$ 为节点几何，$E$ 为边集合。每节点 $v$ 都可以用 $\{\texttt{A},\texttt{B},\ldots ,\texttt{Z}\}$ 的一个子集（可以为空）标记。记 $v$ 上标记的几何为 $L(v)$。定义边 $e=(u,v)$ 的权值 $W(e)$ 为 $L(u)$ 和 $L(v)$ 的相差成都（Hamming 距离），严格地说：

$$W(e)=\left|\{X|X\in L(u)\text{ and }X\notin L(v)\}\cup\{Y|X\notin L(u)\text{ and }X\in L(v)\}\right|.$$

例如：$L(u)=\{\texttt{A},\texttt{B},\texttt{C},\texttt{D},\texttt{E}\}$，而 $L(v)=\{\texttt{B},\texttt{D},\texttt{E},\texttt{F}\}$，则对于 $e=(u,v)$ 来说，$W(e)=|\{\texttt{A},\texttt{C},\texttt{F}\}|=3$。

你的任务是：已知一棵无根树以及所有叶节点的标记集合，求一种**内部节点**的标记方案，使得**所有边的权值的和最小**。

例如给定图 1 中的树以及叶节点标记集合，我们可以得到图 2 或者图 3 的内部节点标记方案（注意，不只这两种，其他的没有列举出来）。图 2 的边权和为 $6$。图 3 的边权和为 $4$。其中图 3 的标记方案是最优的。

![](file://pic1.jpg)

![](file://pic2.jpg)

## 输入格式

第一行为 $N$ 和 $L$，分别表示树的节点数目和叶节点的数目。

树的节点用 $1\sim N$ 编号，接下来 $N-1$ 行，每个两个整数 $u,v$，表示 $u$ 与 $v$ 之间有边。

接着 $L$ 行，每行一个整数和一个字符串，整数表示叶子节点的编号，字符串表示此个点的标记集合，需要注意的是节点的标记集合可以是空集，对应字符串为 `$`。

## 输出格式
 
输出能实现的最小边权和。

```input1
6 4
1 3
2 4
3 4
5 3
4 6
1 AC
2 AB
5 BC
6 B

```

```output1
4
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq N\leq 5\times 10^4$。