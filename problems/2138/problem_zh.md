## 题目描述

话说 Nan 在海边等人，预计还要等上 $M$ 分钟。为了打发时间，他玩起了石子。 Nan 搬来了 $N$堆石子，编号为 $1\sim N$，每堆包含 $A_i$ 颗石子。每 $1$ 分钟，Nan 会在编号在 $[L_i,R_i]$ 之间的石堆中挑出任意 $K_i$ 颗扔向大海（好疼的玩法），如果 $[L_i,R_i]$ 剩下石子不够 $K_i$ 颗，则取尽量地多。为了保留扔石子的新鲜感，Nan 保证任意两个区间 $[L_i,R_i]$ 和 $[L_j,R_j]$ ，不会存在 $L_i\le L_j\ \mathrm{and}\  R_j\le R_i$ 的情况，即任意两段区间不存在包含关系。可是，如果选择不当，可能无法扔出最多的石子，这时 Nan 就会不高兴了。所以他希望制定一个计划，他告诉你他 $m$ 分钟打算扔的区间 $[L_i,R_i]$ 以及 $K_i$ 。现在他想你告诉他，在满足前 $i-1$ 分钟都取到你回答的颗数的情况下，第 $i$ 分钟最多能取多少个石子。

## 输入格式

第一行正整数 $N$ ，表示石子的堆数；

第二行正整数 $x,y,z,P$，$1\le x,y,z\le N$，$1\le P\le 500$；

有等式 $A_{i}=[(i-x)^2+(i-y)^2+(i-z)^2] \mod P$；

第三行正整数 $M$，表示有 $M$ 分钟；

第四行正整数 $K_{1},K_{2},x,y,z,P$，$1\le x,y,z\le 10^3$，$1\le P\le 10^4$；

有等式 $K_{i}=(x\times K_{i-1}+y\times K_{i-2}+z)\mod P$。

接下来 $M$ 行，每行两个正整数 $L_{i},R_{i}$。

## 输出格式

有 $M$ 行，第 $i$ 行表示第 $i$ 分钟最多能取多少石子。

```input1
5
3 2 4 7
3
2 5 2 6 4 9
2 4
1 2
3 5
```

```output1
2
5
5
```

## 数据规模与约定

对于 $100\%$​​​​ 的数据，$1\le N\le 4\times 10^4$，$1\le M\le N$，$1\le L_{i}\le R_{i}\le N$，$1\le A_{i}\le 500$

## 样例说明

石子每堆个数分别为 $0,5,2,5,0$​​​​​​​​​​。

第 $1$​ 分钟，从第 $2$​​​​​​​​​​​ 到第 $4$​​​​​​​​​​​​ 堆中选 $2$​​​​​​​​​​​​ 个；

第 $2$​​ 分钟，从第 $1$​​​ 到第 $2$​​​​​​​​​ 堆中选 $5$​​​​​​​​ 个；

第 $3$ 分钟，从第 $3$​​​​ 到第 $5$​​​​​ 堆中选 $8$​​​​​​​ 个，但最多只能选 $5$​​​​​​ 个。

