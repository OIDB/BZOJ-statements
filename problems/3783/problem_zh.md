## 题目描述

求

$$
\sum_{x=l}^r x \lfloor \frac {ax+c} {b}\rfloor
$$


其中 $a,b,c,l,r$ 均为给定正整数。由于答案可能很大，输出答案 $\bmod {10^9+7}$ 的值。

## 输入格式

第一行五个正整数 $a,b,c,l,r$。

## 输出格式

一个非负整数，表示答案.

```input1
2 3 1 1 3
```

```output1
9
```

## 数据规模与约定

对于 $100\%$ 的数据，$a,b,c,l,r \le 10^9$，$l \le r$。

