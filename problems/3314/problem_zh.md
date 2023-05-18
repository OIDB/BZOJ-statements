

## 题目描述

$N$ 头牛在一个坐标轴上，每头牛有个高度。现给出一个距离值 $D$。

如果某头牛在它的左边，在距离 $D$ 的范围内，如果找到某个牛的高度至少是它的两倍，且在右边也能找到这样的牛的话。则此牛会感觉到不舒服。

问有多少头会感到不舒服。

## 输入格式

第一行两个整数 $N,D$。

接下来 $N$ 行，每行两个整数 $x_i,h_i$，对于任意的 $i\not=j,1\leq i,j\leq N$，都有 $x_i\not=x_j$。

## 输出格式

一行，一个整数，表示答案。

```input1
6 4
10 3
6 2
5 3
9 7
3 6
11 2
```

```output1
2
```

## 样例说明 1

共有 $6$ 头牛，用于判断拥挤的距离为 $4$。奶牛 #$1$ 生活在 $x=10$ 的位置，高度 $h=3$，以此类推。

$x=5$ 和 $x=6$ 位置的奶牛都很拥挤。

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq N\leq 5\times 10^4$，$1\leq x_i,h_i,D\leq 10^9$。

## 题目来源

Silver