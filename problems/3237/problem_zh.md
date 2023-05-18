## 题目描述

给定一个无向连通图和若干个小集合，每个小集合包含一些边，对于每个集合，你需要确定将集合中的边删掉后改图是否保持联通。集合间的询问相互独立。

定义一个图为联通的当且仅当对于任意的两个顶点，都存在一条路径连接它们。

## 输入格式

第一行为两个整数 $n,m$，代表无向图的点数和边数。

下面 $m$ 行，包含两个整数 $u,v$，代表该边连接点 $u,v$。

第 $i + 1$ 行的边的编号为 $i$。保证不存在重边和自环。

下面一行包含一个整数 $k$，表示集合个数。

下面 $k$ 行每行描述一个集合，每行的第一个数为集合中边的个数 $c$，后面 $c$ 个数代表集合内的边。

## 输出格式

对于每个集合，输出一行代表去掉该集合中的边后图是否联通，如果联通输出 `Connected`，否则输出 `Disconnected`。

```input1
4 5
1 2
2 3
3 4
4 1
2 4
3
1 5
2 2 3
2 1 2
```

```output1
Connected
Disconnected
Connected
```

## 数据规模与约定

* 对于 $100\%$ 的数据，$n \leq 10^5$，$m \leq 2 \times 10^5$，$k \leq 10^5$。

## 题目来源

没有写明来源