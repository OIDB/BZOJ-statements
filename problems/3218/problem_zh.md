## 题目描述

题目名称是吸引你点进来的。

从前有 $n$ 个方格排成一行。从左至右依次编号为 $1,2,\cdots,n$。

有一天思考熊想给这 $n$ 个方格染上黑白两色。

第 $i$ 个方格上有 $6$ 个属性：$a_i,b_i,w_i,l_i,r_i,p_i$。

如果方格 $i$ 染成黑色就会获得 $b_i$ 的好看度。

如果方格 $i$ 染成白色就会获得 $w_i$ 的好看度。

但是太多了黑色就不好看了。

如果方格 $i$ 是黑色，并且存在一个白色方格 $j$ 使得：

$$1 \leq j < i,l_i \leq a_j \leq r_i$$

那么方格 $i$ 就被称为奇怪的方格。

如果方格 $i$ 是奇怪的方格，就会使总好看度减少 $p_i$。

也就是说对于一个染色方案，好看度为：

$$\sum\limits_{\text{方格 }i\text{ 为黑色}} b_i + \sum\limits_{\text{方格 }i\text{ 为白色}} w_i - \sum\limits_{\text{方格 }i\text{ 为奇怪的方格}} p_i$$

现在给你 $n,a,b,w,l,r,p$，问所有染色方案中**最大**的好看度是多少。

## 输入格式

第一行一个**正整数** $n$。

接下来 $n$ 行中第 $i$ 行有用空格隔开的 $6$ 个**非负整数**以此表示 $a_i,b_i,w_i,l_i,r_i,p_i$。

## 输出格式

一个非负整数表示所有染色方案中最大的好看度。

```input1
10
0 1 7 3 9 2
7 4 0 9 10 5
1 0 4 2 10 2
7 9 1 5 7 2
6 3 5 3 6 2
6 6 4 1 8 1
6 1 6 0 6 5
2 2 5 0 9 3
5 1 3 0 2 5
5 6 7 1 1 2
```

```output1
55
```

## 样例说明

最优染色方案为：白黑白黑白黑白白白白。

可以发现只有方格 $6$ 为奇怪的方格。

所以好看度为：$w_1+b_2+w_3+b_4+w_5+b_6+w_7+w_8+w_9+w_{10}-p_6=7+4+4+9+5+6+6+5+3+7-1=55$。

## 数据规模与约定

设 $maxA$ 为 $a,l,r$ 中的最大值，$maxV$ 为 $b,w$ 中的最大值，$maxP$ 为 $p$ 中的最大值。对于各个测试点：

|测试点编号|$n$|$maxA$|$maxV$|$maxP$|
|:-----:|:-----:|:-----:|:-----:|:-----:|
|$1$|$n = 5$|$maxA \leq 10$|$maxV \leq 10$|$maxP \leq 10$|
|$2$|$n = 20$|$maxA \leq 40$|$maxV \leq 40$|$maxP \leq 40$|
|$3$|$n = 20$|$maxA \leq 40$|$maxV \leq 40$|$maxP \leq 40$|
|$4$|$n = 5000$|$maxA \leq 10$|$maxV \leq 2 \times 10^5$|$maxP \leq 10^5$|
|$5$|$n = 5000$|$maxA \leq 10$|$maxV \leq 2 \times 10^5$|$maxP \leq 3 \times 10^5$|
|$6$|$n = 200$|$maxA \leq 10^9$|$maxV \leq 2 \times 10^5$|$maxP \leq 2 \times 10^5$|
|$7$|$n = 300$|$maxA \leq 10^9$|$maxV \leq 2 \times 10^5$|$maxP \leq 2.2 \times 10^5$|
|$8$|$n = 500$|$maxA \leq 10^9$|$maxV \leq 2 \times 10^5$|$maxP \leq 4 \times 10^5$|
|$9$|$n = 5000$|$maxA \leq 5000$|$maxV \leq 2 \times 10^5$|$maxP \leq 1.5 \times 10^5$|
|$10$|$n = 5000$|$maxA \leq 10^9$|$maxV \leq 2 \times 10^5$|$maxP \leq 3 \times 10^5$|

每个测试点时间限制：$\text{2s}$

每个测试点内存限制：$\text{48MB}$