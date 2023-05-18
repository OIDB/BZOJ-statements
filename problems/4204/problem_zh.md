## 题目描述

有 $M$ 个球，一开始每个球均有一个初始标号，标号范围为 $1\sim N$ 且为整数，标号为 $i$ 的球有 $a_i$ 个，并保证 $\sum_{i=1}^N a_i = M$。

每次操作等概率取出一个球（即取出每个球的概率均为 $\frac{1}{M}$），若这个球标号为 $k(k < N)$，则将它重新标号为 $k + 1$；若这个球标号为 $N$，则将其重标号为 $1$。（取出球后并不将其丢弃）

现在你需要求出，经过 $K$ 次这样的操作后，每个标号的球的期望个数。

## 输入格式

第 $1$ 行包含三个正整数 $N,M,K$，表示了标号与球的个数以及操作次数。

第 $2$ 行包含 $N$ 个非负整数 $a_i$，表示初始标号为 $i$ 的球有 $a_i$ 个。

## 输出格式

包含 $N$ 行，第 $i$ 行为标号为 $i$ 的球的期望个数，四舍五入保留 $3$ 位小数。

## 样例
```input1
2 3 2
3 0
```
```output1
1.667
1.333
```
## 样例说明

第一次操作后，由于标号为 $2$ 球个数为 $0$，所以必然是一个标号为 $1$ 的球变为标号为 $2$ 的球。所以有 $2$ 个标号为 $1$ 的球，有 $1$ 个标号为 $2$ 的球。第二次操作后，有 $\frac{1}{3}$ 的概率标号为2的球变为标号为 $1$ 的球（此时标号为 $1$ 的球有 $3$ 个），有 $\frac{2}{3}$ 的概率标号为 $1$ 的球变为标号为 $2$ 的球（此时标号为 $1$ 的球有 $1$ 个），所以标号为 $1$ 的球的期望个数为 $\frac{1}{3}\times 3+\frac{2}{3}\times 1 = \frac{5}{3}$。同理可求出标号为 $2$ 的球期望个数为 $\frac{4}{3}$。

## 数据规模与约定

对于 $100\%$ 的数据：$N \le 10^3$，$M \le 10^8$，$K \le 2147483647$。