## 题目描述

小 C 最近学了很多最小生成树的算法，Prim 算法、Kruskal 算法、消圈算法等等。

正当小 C 洋洋得意之时，小 P 又来泼小 C 冷水了。小 P 说，让小 C 求出一个无向图的次小生成树，而且这个次小生成树还得是严格次小的，也就是说：如果最小生成树选择的边集是 $E_M$，严格次小生成树选择的边集是 $E_S$，那么需要满足：

$$\sum_{e \in E_M}\operatorname{value}(e) < \sum_{e \in E_S}\operatorname{value}(e)$$

（$\operatorname{value}(e)$ 表示边 $e$ 的权值）

这下小 C 蒙了，他找到了你，希望你帮他解决这个问题。

## 输入格式

第一行包含两个整数 $n$ 和 $m$，表示无向图的点数与边数。

接下来 $m$ 行，每行三个数 $x, y, z$ 表示，点 $x$ 和点 $y$ 之间有一条边，边的权值为 $z$。

## 输出格式

包含一行，仅一个数，表示严格次小生成树的边权和（数据保证必定存在严格次小生成树）。

```input1
5 6
1 2 1
1 3 2
2 4 3
3 5 4
3 4 3
4 5 6
```

```output1
11
```

## 数据规模与约定

数据中无向图无自环；

- 对于 $50\%$ 的数据，$n \le 2 \times 10^3$，$m \le 3 \times 10^3$；
- 对于 $80\%$ 的数据，$n \le 5 \times 10^4$，$m \le 10^5$；
- 对于 $100\%$ 的数据，$n \le 10^5$，$m \le 3 \times 10^5$，边权值非负且不超过 $10^9$。