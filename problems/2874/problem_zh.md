## 题目描述

有一个 $n\times m$ 的矩阵，初始全为 $0$​。

对其进行 $k$ 次矩阵加，矩阵加操作 **全部完成** 后 **强制在线** 回答 $q$ 次矩阵和。

## 输入格式

第一行四个整数 $n,m,k,q$。

接下来 $k$ 行，每行五个整数 $x_1,x_2,y_1,y_2,s$ 表示对以 $(x_1,y_1)$ 为左上角，$(x_2,y_2)$ 为右下角的矩阵的每个位置加上 $s$。

接下来 $q$ 行，每行两个整数 $x,y$，询问的矩阵以如下方式进行，记 $c$​ 为上一个问题的答案，那么：

$x_1=c\bmod n +1,x_2=(c+x)\bmod n+1$，若 $x_1>x_2$ 则交换 $x_1,x_2$；

$y_1=c\bmod m+1,y_2=(c+x)\bmod m+1$，若 $y_1>y_2$ 则交换 $y_1,y_2$。

询问以 $(x_1,y_1)$​ 为左上角，$(x_2,y_2)$ 为右下角的矩阵的和。

保证答案小于 $2^{64}$。

## 输出格式

共 $q$ 行，对于每个询问输出一行答案。

```input1
4 5 3 3
1 3 2 2 7
2 4 2 3 5
1 4 4 5 6
1 2
0 3
2 2
```

```output1
24
12
46
```

```input2
5 5 5 5
1 1 1 3 242
1 4 4 5 83
3 5 3 3 221
2 2 1 3 254
5 5 2 2 105
0 1
0 4
2 1
1 3
0 1
```

```output2
484
0
992
442
304
```

## 样例解释

对于样例 #1，三次询问的矩阵左上角与右下角坐标分别是：

$(1,1),(2,3)$；

$(1,3),(1,5)$；

$(1,3),(3,5)$。

## 数据规模与约定

对于 $100\%$​ 的数据，$1\leq n,m\leq 10^8$，$1\leq k\leq 4\times 10^4$，$1\leq q\leq 10^5$。
