## 题目描述

一天 rin 来到了一个遥远的都市。这个都市有 $n$ 个建筑，编号从 $1$ 到 $n$，其中市中心编号为 $1$，这个都市有 $m$ 条双向通行的街道，每条街道连接着两个建筑，其中某些街道首尾相连连接成了一个环。

rin 通过长时间的走访，已经清楚了这个都市的两个特点：
1. 从市中心出发可以到达所有的建筑物。
2. 任意一条街道最多存在与一个简单环中。

令 rin 心花怒放的是，每个建筑物都会有拉面售卖。拉面有很多不同的种类，但对于 rin 而言只有油腻程度的不同，因此我们把油腻程度相同的拉面看做同一种拉面。

由于不同建筑物的拉面的油腻程度可能不同，我们用一个正整数来表示拉面的油腻程度。

要知道，拉面可是 rin 的最爱，但是现在到了下班高峰期，都市的交通变得非常的堵塞。rin 只能通过没有被堵死的街道通行，去品尝所在建筑物的拉面。

现在 rin 想知道，如果她正在编号为 $x$ 的建筑物，那么在从市中心到 $x$ 的所有简单路径经过的街道都被堵死的情况下，rin 可以品尝到的拉面中（注意没有出现的拉面是不能算在里面的）：
1. 油腻程度 $\leq y$ 且品尝次数为奇数次的拉面有多少种？
2. 油腻程度 $\leq y$ 且品尝次数为偶数次的拉面有多少种？

##  输入格式

第一行两个正整数 $n,m$，含义如题所示第二行一共 $n$ 个正整数，第 $i$ 个数 $a_i$ 表示第 $i$ 个建筑物出售的拉面的油腻程度。  
接下来 $m$ 行，每行两个正整数 $x,y$，表示在建筑物 $x,y$ 之间有一条双向通行的街道。
接下来一行一个正整数 $q$，表示询问个数。  
接下来 $q$ 行每行三个非负整数 $ty,x,y,x$ 表示询问的建筑物编号，$y$ 表示油腻程度的限制，$ty=0$ 时表示询问偶数，$ty=1$ 表示询问奇数。


## 输出格式

一共 $q$ 行，对于每个询问输出一个答案。

```input1
10 12
1 10 4 5 2 10 1 8 4 8
1 2
1 3
1 4
2 5
4 6
4 7
7 8
2 9
8 10
1 6
8 10
4 7
10
0 3 9
1 7 6
0 5 2
1 10 9
0 5 7
1 7 4
0 7 3
1 2 7
0 3 4
0 3 8
```

```output1
0
1
0
1
0
1
0
2
0
0
```

## 数据规模与约定


对于 $100\%$ 的数据，$n \leq 10^5$，$m \leq 1.5 \times 10^5$，$q \leq 10^5$，$a_i \leq 10^6$，$1 \leq x \leq n$，$0 \leq y \leq 10^6$。