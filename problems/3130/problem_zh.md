## 题目描述

Alice 和 Bob 在图论课程上学习了最大流和最小费用最大流的相关知识。最大流问题：给定一张有向图表示运输网络，一个源点 $s$ 和一个汇点 $t$，每条边都有最大流量。一个合法的网络流方案必须满足：

1. 每条边的实际流量都不超过其最大流量且非负；
2. 除了源点 $s$ 和汇点 $t$ 之外，对于其余所有点，都满足该点总流入流量等于该点总流出流量；

而  $s$ 点的净流出流量等于 $t$ 点的净流入流量，这个值也即该网络流方案的总运输量。最大流问题就是对于给定的运输网络，求总运输量最大的网络流方案。上图表示了一个最大流问题。对于每条边，右边的数代表该边的最大流量，左边的数代表在最优解中，该边的实际流量。需要注意到，一个最大流问题的解可能不是唯一的。 对于一张给定的运输网络，Alice 先确定一个最大流，如果有多种解，Alice 可以任选一种；之后 Bob 在每条边上分配单位花费（单位花费必须是非负实数），要求所有边的单位花费之和等于 $p$。总费用等于每一条边的实际流量乘以该边的单位花费。需要注意到，Bob 在分配单位花费之前，已经知道 Alice 所给出的最大流方案。现茌 Alice 希望总费用尽量小，而 Bob 希望总费用尽量大。我们想知道，如果两个人都执行最优策略，最大流的值和总费用分别为多少。

## 输入格式

第一行三个整数 $n,m,p$。$n$ 表示给定运输网络中节点的数量，$m$ 表示有向边的数量， $p$ 的含义见问题描述部分。为了简化问题，我们假设源点 $s$ 是点  $1$，汇点 $t$ 是点 $n$ 。 接下来 $m$ 行，每行三个整数 $a,b,c$，表示有一条从点 $a$ 到点 $b$ 的有向边，其最大流量是 $c$。

## 输出格式

第一行一个整数，表示最大流的值。第二行一个实数，表示总费用。建议选手输出四位以上小数。



```input1
3 2 1
1 2 10
2 3 15
```



```output1
10
10.0000
```

## 样例说明

对于 Alice，最大流的方案是固定的。两条边的实际流量都为 $10$。对于 Bob，给第一条边分配 $0.5$ 的费用，第二条边分配 $0.5$ 的费用。总费用为：$10\times 0.5+10\times 0.5=10$。可以证明不存在总费用更大的分配方案。

## 数据规模和约定

对于 $20\%$ 的测试数据，所有有向边的最大流量都是$1$。

对于 $100\%$ 的测试数据，$n \le 100，m \le 10^3$，所有点的编号在 $1 \dots n$ 范围内。$1 \le $ 每条边的最大流量 $\le  5 \times 10^4 $。$1 \le p \le 10$。给定运输网络中不会有起点和终点相同的边。
