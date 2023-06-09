## 题目描述

你在一家 IT 公司为大型写字楼或办公楼（offices）的计算机数据做备份。然而数据备份的工作是枯燥乏味的，因此你想设计一个系统让不同的办公楼彼此之间互相备份，而你则坐在家中尽享计算机游戏的乐趣。

已知办公楼都位于同一条街上。你决定给这些办公楼配对（两个一组）。每一对办公楼可以通过在这两个建筑物之间铺设网络电缆使得它们可以互相备份。然而，网络电缆的费用很高。当地电信公司仅能为你提供 $k$ 条网络电缆，这意味着你仅能为 $k$ 对办公楼（或总计 $2k$ 个办公楼）安排备份。任一个办公楼都属于唯一的配对组（换句话说，这 $2k$ 个办公楼一定是相异的）。

此外，电信公司需按网络电缆的长度（公里数）收费。因而，你需要选择这 $k$ 对办公楼使得电缆的总长度尽可能短。换句话说，你需要选择这 $k$ 对办公楼，使得每一对办公楼之间的距离之和（总距离）尽可能小。

下面给出一个示例，假定你有 $5$ 个客户，其办公楼都在一条街上，如下图所示。这 $5$ 个办公楼分别位于距离大街起点 $1\text{km}, 3\text{km}, 4\text{km}, 6\text{km}$ 和 $12\text{km}$ 处。电信公司仅为你提供 $k=2$ 条电缆。

![](https://hydro.org.cn/d/bzoj/p/1150/file/pic1.png)

上例中最好的配对方案是将第 $1$ 个和第 $2$ 个办公楼相连，第 $3$ 个和第 $4$ 个办公楼相连。这样可按要求使用 $k=2$ 条电缆。第 $1$ 条电缆的长度是 $3\text{km}-1\text{km}=2\text{km}$，第 $2$ 条电缆的长度是 $6\text{km}-4\text{km}=2\text{km}$。这种配对方案需要总长 $4\text{km}$ 的网络电缆，满足距离之和最小的要求。

## 输入格式

输入的第一行包含整数 $n$ 和 $k$，其中 $n$ 表示办公楼的数目，$k$ 表示可利用的网络电缆的数目。

接下来的 $n$ 行每行仅包含一个整数 $s$, 表示每个办公楼到大街起点处的距离。这些整数将按照从小到大的顺序依次出现。

## 输出格式

输出应由一个正整数组成，给出将 $2k$ 个相异的办公楼连成 $k$ 对所需的网络电缆的最小总长度。

```input1
5 2
1
3
4
6
12
```

```output1
4
```

## 数据规模与约定

对于 $100\%$ 的数据，$2 \le n \le 10^5, 1 \le k \le \dfrac{n}{2}, 0 \le s \le 10^9$