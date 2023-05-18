## 题目描述
你被雇佣升级一个旧果汁加工厂的橙汁运输系统。系统有管道和节点构成。每条管道都是双向的，且每条管道的流量都是 $1$ 升每秒。管道可能连接节点，每个节点最多可以连接 $3$ 条管道。节点的流量是无限的。节点用整数 $1$ 到 $n$ 来表示。在升级系统之前，你需要对现有系统进行分析。对于两个不同节点 $s$ 和 $t$，$s - t$ 的流量被定义为：当 $s$ 为源点，$t$ 为汇点，从 $s$ 能流向 $t$ 的最大流量。以下面的第一组样例数据为例，$1 \sim 6$ 的流量为 $3$，$1 \sim 2$ 的流量为 $2$。计算每一对满足 $a \lt b$ 的节点 $a \sim b$ 的流量的和。

## 输入格式
第一行包括 $2$ 个整数 $n$ 和 $m$——节点数和管道数。  
接下来 $m$ 行，每行包括两个相异整数 $a$，$b$，表示一条管道连接节点 $a$，$b$。
每个节点最多连接 $3$ 条管道，每对节点最多被一条管道连接。

## 输出格式
输出一个整数——每对满足 $a \lt b$ 的节点 $a \sim b$ 的流量之和。

```input1
6 8
1 3
2 3
4 1
5 6
2 6
5 1
6 4
5 3
```

```output1
36
```

## 数据范围与约定
对于 $100 \%$ 的数据，$2 \le n \le 3000$，$0 \le m \le 4500$，$1 \le a, b \le n$。