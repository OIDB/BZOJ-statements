## 题目描述

给一个 $n \times n$ 的地图，每个格子有一个价格，找一个矩形区域，使其价格总和位于 $[k,2k]$。

## 输入格式

输入$k,n$和一个 $n \times n$ 的地图。

## 输出格式

输出矩形的左上和右下的列-行坐标或 `NIE`。

```input1
4 3
1 1 1
1 9 1
1 1 1
```

```output1
NIE
```

```input2
8 4
1 2 1 3
25 1 2 1
4 20 3 3
3 30 12 2
```

```output2
2 1 4 2
```

## 数据规模与约定

$n < 2000, 1 \leq k \le 10^9$。

 每个价格都是不大于 $2 \times 10^9$ 的非负整数。

