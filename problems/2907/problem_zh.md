## 题目描述

某蒟蒻被虐爆太多于是去拜访神犇，有 $n$ 个神犇生活在一维世界，住在数轴上某点，每个神犇都有个互不相同的坐标值 $x_i$，神犇有神力，可以在一维世界任意移动，但是蒟蒻不行，蒟蒻一开始在某个神犇处，神犇借了他一点神力用，蒟蒻可以借助神力向左（数轴负方向）移动任意距离 $l$ 次，向右（数轴正方向）移动任意距离 $n-l-1$ 次，移动耗时为两点之间的距离差的绝对值。他移动完毕后到达一个神犇的位置时就视作他拜访了这个神犇，当他成功拜访完 $n$ 个神犇后他就可以从蒟蒻进化成弱菜。他希望快点成为弱菜，所以希望你能告诉他,他最快需要多少时间成为弱菜？由于今天是最后一天就不需要给出方案了。

## 输入格式

第一行 $3$ 个数字 $n,l,s$ 表示神犇数，蒟蒻可以向左移动的次数和蒟蒻所在位置的神犇编号。

第二行 $n$ 个升序排列的数字，第 $i$ 个数字表示第 $i$ 个神犇所在的坐标大小 $x_i$。

## 输出格式

一个数，蒟蒻成为弱菜的最短耗时。如果蒟蒻无法成为弱菜是天命就输出 `-1`。

```input1
5 2 2
0 10 11 21 22
```

```output1
33
```
## 提示

蒟蒻可以向左移动 $2$ 次，向右移动 $2$ 次。现在在 $2$ 号神犇处坐标为 $10$，他先向左移动一次，访问 $1$ 号神犇，移动耗时 $10$，然后向右移动访问 $3$ 号神犇，移动耗时 $11$，向右移动访问 $5$ 号神犇，移动耗时 $11$，然后向左移动访问 $4$号神犇，移动耗时 $1$，总耗时 $33$，总公共向左移动 $2$ 次，向右移动 $2$ 次。

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n\le10^5$，$0=x_1<x_2<\dots<x_{n-1}<x_n\le10^9$。
