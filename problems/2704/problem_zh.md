## 题目描述

有一个 $n \times m$ 的格子地图，地图上的格子有些是障碍，不能通过，有些不是障碍，有一个快乐程度，从每个格子可以移向上下左右四个格子。

小月想从 $[1,1]$ 格出发，旅游一些格子并回到 $[1,1]$ 格，旅游的快乐程度等于经过的所有格子的快乐程度之和，小月想使得旅游的快乐程度之和尽可能大。

注意：
1. 保证 $[1,1]$ 格不是障碍
2. 除 $[1,1]$ 格外不能重复走过同一格
3. $[1,1]$ 格的快乐程度只算一次
4. 快乐程度可能是负数
5. 若不能从 $[1,1]$ 格出去并回来，则小月不会进行此次旅游。
6. 若旅游的快乐程度为负数，则小月不会进行此次旅游。
7. 若小月不会进行旅游，则旅游快乐程度为 $0$。



## 输入格式

第一行两个正整数 $n,m$ 。

接下来 $n$ 行，每行 $m$ 个整数，第 $i$ 行第 $j$ 列的数为 $a_{i,j}$。当 $a_{i,j}=0$ 时表示此格是障碍，否则表示快乐程度。




## 输出格式

仅一行一个数，表示最大的旅游快乐程度。

```input1
3 3
1 9 -1
-7 0 8
-1 -1 -1
```

```output1
7
```

## 数据规模与约定

- 对于 $100\%$ 的数据满足 $n,m \le 12$，$-(10^4) \le a[i][j] \le 10^4$。