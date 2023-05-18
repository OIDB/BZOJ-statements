## 题目描述

据说，加勒比海盗每次抢劫完，如果有金银珠宝等贵重物品，都会以特殊的仪式分宝。

他们首先将珠宝装在一个个边长为 $1$ 的土陶立方体中，并在盖子上标记出珠宝的价值 $v$。然后将这些盒子排列成一个长为 $l$，宽为 $w$ 的矩形（如果珠宝不够，可能会用空的土陶盒占据空位，并在盖子上标记价值为 $0$），第 $i$ 行第 $j$ 列的土陶盒上标记的价值为 $v_{i,j}$（其中 $0\le i\lt w$，$0\le j\lt l$，左下角的土陶盒所在位置为第一行第一列）。

海盗们按照功劳的大小，决定分宝的顺序，被轮到选取珠宝的海盗将被发给一个底面为 $m\times n$ 的矩形，高为 $h$ 的木箱子，并要求用这个木箱子来装所选土陶盒，最后盖上木箱盖子。土陶盒的选取需要分批选取，要求每批土陶盒为一个等同于木箱底面的紧挨着的矩形区域，且木箱长为 $m$ 的边必须与土陶盒摆成矩形时长为 $w$ 的边平行。被选走的土陶盒所在位置在被选走后马上由空土陶盒填充。

海盗从土陶盒摆成的矩形底部正中出发，即从第一行的第 $\lfloor \frac{w}{2}\rfloor$ 列的土陶盒的右下角出发，向上沿着据土陶盒摆成的矩形区域的最左边 $\lfloor \frac{w}{2}\rfloor$ 的直线前进。如图中粗线箭头所示。

设第 $k$ 批被选取的区域的左下角为第 $i_k$ 行第 $j_k$ 列的土陶盒，$j_k$ 必须满足 $\lfloor \frac{m}{2}+j_k-\frac{w}{2}\rfloor \lt a$，其中 $k\ge 1$；

且当 $j_k = j_{k-1}$ 的时候，$i_k$ 必须满足 $i_k-i_{k-1} \ge d_1$，当 $j_k \ne j_{k-1}$ 时，$i_k$ 必须满足 $i_k - i_{k-1} \ge d_2$，其中 $k\ge 2$。

![pic1.png](file://pic1.png)

## 输入格式

第一行包括 $8$ 个正整数，这些正整数之间用一个空格隔开，这 $8$ 个正整数依次为 $l$，$w$，$m$，$n$，$h$，$a$，$d_1$，$d_2$。

从第二行到第 $l+1$ 行，每行有 $w$ 个整数，不妨将输入文件中第 $i+1$ 行，第 $j$ 列的整数记做 $v_{i,j}$（$1\lt j\lt w$，$1\lt i\lt l$），分别表示土陶盒上标记的珠宝价值，同一行的整数之间用一个空格隔开。

需注意的是：输入时 $v_{i,j}$ 是从左上角的土陶盒开始，但在求解时左下角的那个土陶盒为第 $1$ 行第 $1$ 列的土陶盒。

## 输出格式

输出文件中的第一行为一个整数，是最多能得到的珠宝总价值 $Total$

```input1
10 12 3 2 3 5 2 3
0 0 0 1 0 1 1 1 9 1 1 1
1 1 2 1 1 1 0 0 8 2 1 8
1 0 1 0 1 6 1 1 0 0 1 1
1 1 2 1 2 1 1 1 3 1 1 1
0 1 0 1 1 1 2 1 6 0 2 1
1 1 0 1 0 1 1 2 1 1 1 0
1 0 1 1 1 0 1 0 1 1 0 1
1 1 0 1 1 1 9 0 0 1 1 1
0 0 1 0 1 2 1 9 1 1 0 1
0 1 1 1 1 1 9 1 1 1 1 1
```

```output1
59
```

## 数据规模与约定


对于 $100\%$ 的数据：

- $1\lt l, w \lt 2000$；
- $1\lt m, n\lt 200$；
- $1\lt h\lt 20$；
- $1\lt a\lt 2000$；
- $1\lt d_1, d_2\lt 2000$；
- $0\lt v_{i,j}\lt 255$；
- 数据保证 $d_1,d_2\ge n$。