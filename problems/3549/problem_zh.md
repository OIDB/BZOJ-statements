## 题目描述

给定 $n$ 个积木，编号为 $1 \dots n$，每个积木高度为 $1$，宽度为 $w_i$，你可以把若干个积木放在一层上，堆成若干层，要求满足两个条件：

1. 对于任意一层的积木，他的宽度之和要小于等于他下面那一层的积木（最底层除外）。
2. 不允许编号小的放在编号大的的积木上面。

让你求最多能够堆多少层。

## 输入格式

第一行一个数 $n$。

第二行 $n$ 个整数 $w_i$。

## 输出格式

一行一个整数表示答案。

```input1
3
1 2 3
```
```output1
2
```

## 提示

$n \le 10^5,~w_i \le 10^4$

## 题目来源

By Sbullet
