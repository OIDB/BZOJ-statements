## 题目描述

已丢失

## 输入格式

本题有多组输入。

第一行有一个正整数 $T$，表示数据组数，然后是 $T$ 组数据。

每组数据由 $5$ 行组成，每行有 $6$ 个字符，使用 $5$ 中字符描述矩阵：`.`、`#`、`3`、`S`、`T`。

- `.` 表示空地
- `#` 表示障碍物
- `3` 表示苹果树
- `S` 表示小 Y
- `T` 表示小偷

每组数据有且只有 $1$ 个 `S` 和 `T`，并且其所在的位置一定是一个空地。每组数据至少有一半的位置是障碍物，每组数据的最后都有一个空行。

## 输出格式

每组数据输出一个整数表示小偷最多能够得到的苹果数

```input1
3 
T3333.
#####S
######
######
######

####..
.3.3..
33.T.S
######
######

##3###
##.##3
TS3###
##.###
##3###

```
```output1
9
12
0
```

## 样例说明

对于第三个样例，小 Y 可以永远停留在他右边的苹果树上，那么小偷就再也偷不到苹果了，此时 Game Over。

## 数据范围

对于 $100\%$ 的数据：$T \leq 20$。

## 题目来源

Acm2005 成都