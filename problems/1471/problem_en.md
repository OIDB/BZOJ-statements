## 题目描述

给出一个 $n$ 个结点的有向无环简单图。给出 $4$ 个不同的点 $a,b,c,d$，定义不相交路径为两条路径，两条路径的起点分别为 $a$ 和 $c$，对应的两条路径的终点为 $b$ 和 $d$，要求满足这两条路径不相交，即两条路径上没有公共的点。 现在要求不相交路径的方案数。

## 输入格式

第一行为 $n,m$，表示这个有向无环图有 $n$ 个节点，$m$ 条边。 接下来 $m$ 行，每行两个整数 $x,y$，表示 $x$ 至 $y$ 有一条有向边。 接下来一行四个数 $a,b,c,d$，意义如题中所述。

## 输出格式

输出为一行，即答案（方案数）。

```input1
5 6
1 5
1 3
2 5
2 4
5 3
5 4
1 3 2 4
```

```output1
3
```

## 数据规模与约定

对于 $100\%$ 的数据，$n\leq 150$。