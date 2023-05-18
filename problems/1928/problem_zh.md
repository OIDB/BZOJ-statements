## 题目背景

众所周知，在太阳系外围有一圈小行星带，而太阳系中离小行星带最近的 Neptune 往往面临着遭受小行星轰击的威胁。突然某天，Neptune 上的天文台发现有一群小行星有 $k$ 颗气势汹汹的袭来。作为 Neptune 的天文部长的小 t 想知道这些小行星分别要多久会撞到 Neptune。你能够帮助他吗？

## 题目描述

这些小行星的运行遵循以下一些规则：

- 任意两颗小行星不会经过完全一样的路径，但有可能有绝大部分相同；
- 对于某些小行星有可能受到其路径上的比较大的矮行星的引力作用，而围绕某个区域转圈；
- 由于力的方向性，所以所有路径方向都是一定的；
- 我们把空间中小行星可能经过的地方抽象成一个个点，并标号。共有 $N$ 个点；
- 由于我们只关心其路径长度，所以并不给出这些点的具体坐标；
- 两点间有可能有多条直接路径。任意两点间共有 $M$ 条这样的路径；
- 每课小行星在一个单位时间中会运动一个天文单位。且都会在当前的从起点到 Neptune 的最短路径上运行；
- 每颗小行星对于我们来说都是一样的。

请你编程求出所有小行星从起点（同一个起点）到达 Neptune 的所需花费的时间。

## 输入格式

第一行: $5$ 个用空格隔开的整数：$N,M,K,S,T$，表示有 $N$ 个点 $M$ 条边 $K$ 个小行星，起点的标号为 $S$，Neptune 的标号为 $T$。
接下来 $M$ 行每行 $3$ 个大于 $0$ 的整数，表示每条边的起点标号和终点标号以及这条边的长度。

## 输出格式

共有 $K$ 行，每行一个整数，表示一颗小行星所要花费的时间。

```input1
6 6 2 1 6
1 2 1
2 4 1
4 5 1
5 6 1
2 3 1
3 5 1
```

```output1
4
4
```

## 数据规模与约定

$1 \le N \le 1 \times 10^4,1 \le M \le 5 \times 10^5,1 \le K \le 100.$  
对于所有数据在给定的数据范围内阶梯增长。
