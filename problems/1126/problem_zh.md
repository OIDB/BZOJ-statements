## 题目描述

给一个 $n \times m$ 地图，计算从 $(n,1)$【注：左下角】到第 $x$ 列的第 $y$ 行的路径条数$\bmod k$，走过的点不能再走，转弯只能向右转。

## 输入格式

第一行输入 $n,m,k$。

第二行输入$x,y$，注意这里是 $x$ 列 $y$ 行。

以下 $n$ 行 $m$ 列的字符矩阵 `+` 表示可以走，`*` 表示障碍。

## 输出格式

答案 $\bmod k$

```input1
3 5 10
4 2
+++++
++*++
++++*
```

```output1
2
```

## 数据规模与约定

$1 \leq n,m \leq 100, 1 \leq k \leq 10^9$。