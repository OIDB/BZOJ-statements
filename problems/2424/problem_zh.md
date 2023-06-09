## 题目描述

某公司估计市场在第 $i$ 个月对某产品的需求量为 $U_i$ ，已知在第 $i$ 月该产品的订货单价为 $d_i$ ，上个月月底未销完的单位产品要付存贮费用 $m$ ，假定第一月月初的库存量为零，第 $n$ 月月底的库存量也为零，问如何安排这 $n$ 个月订购计划，才能使成本最低？

每月月初订购，订购后产品立即到货，进库并供应市场，于当月被售掉则不必付存贮费。假设仓库容量为$S$ 。

## 输入格式

第 $1$ 行：$n, m, S$ 。

第 $2$ 行：$U_1 , U_2 , \cdots , U_i , \cdots , U_n$ 。

第 $3$ 行：$d_1 , d_2 , \cdots , d_i , \cdots , d_n$ 。

## 输出格式

只有 $1$ 行，一个整数，代表最低成本。

```input1
3 1 1000
2 4 8
1 2 4
```

```output1
34
```

## 数据规模与约定

对于 $100\%$ 的数据，$0\le n \le 50 , 0\le m \le 10 , 0\le S \le 10000 , 0\le U_i \le 10000 , 0\le d_i \le 100$ 。

## 题目来源

$\text{HAOI2010 Day1}$ 。
