## 题目描述

![](file://pic1.jpg)

令 $T$ 为一个有根树，$S$ 为 $T$ 的复制得到的树。

我们合并 $S$ 和 $T$ 对应的叶子节点，这样就得到了一个新的图，我们称之为 tree-mirrored graph。

写一个程序验证一个给定的图是否是 tree-mirrored graph。

## 输入格式

第一行两个整数 $n$ 和 $m$ 表示给定图的点数与边数。

接下来 $m$ 行，每行两个数 $u$ 和 $v$ 表示图中的一条边，保证无重边与自环。

## 输出格式

输出一个字符串 `YES` 或 `NO` 表示这个图是不是 tree-mirrored graph。

## 样例输入

```plain
7 7
1 2
2 3
3 4
4 5
5 6
6 7
7 1
```

## 样例输出

```plain
NO
```

## 数据规模与约定

对于 $30\%$ 的数据，$3 \le n,m \le 300$。

对于 $60\%$ 的数据，$3 \le n,m \le 3.5\times 10^3$。

对于所有数据，$3 \le n,m \le 10^5$。
