## 题目描述

lqp 在为出题而烦恼，他完全没有头绪，好烦啊……

他首先想到了整数拆分。整数拆分是个很有趣的问题。给你一个正整数 $n$，对于 $n$ 的一个整数拆分就是满足任意 $m>0$，$a_1,a_2,a_3\dots,a_m>0$，且 $a_1+a_2+a_3+\dots+a_m=n$ 的一个有序集合。

通过长时间的研究我们发现了计算对于 $n$ 的整数拆分的总数有一个很简单的递推式，但是因为这个递推式实在太简单了，如果出这样的题目，大家会对比赛毫无兴趣的。

然后 lqp 又想到了斐波那契数。定义 $f_0=0,f_1=1,f_n=f_{n-1}+f_{n-2} (n>1)$，$f_n$ 就是斐波那契数的第 $n$ 项。但是求出第 $n$ 项斐波那契数似乎也不怎么困难……

lqp 为了增加选手们比赛的欲望，于是绞尽脑汁，想出了一个有趣的整数拆分，我们暂且叫它：整数的 lqp 拆分。和一般的整数拆分一样，整数的 lqp 拆分是满足任意 $m>0$，$a_1 ,a_2 ,a_3\dots a_m>0$，且 $a_1+a_2+a_3+\dots+a_m=n$ 的一个有序集合。

但是整数的 lqp 拆分要求的不是拆分总数，相对更加困难一些。对于每个拆分，lqp 定义这个拆分的权值 $f_{a_1}f_{a_2}\dots f_{a_m}$，他想知道对于所有的拆分，他们的权值之和是多少？

由于这个数会十分大，lqp 稍稍简化了一下题目，只要输出对于 $n$ 的整数 lqp 拆分的权值和 $\bmod 10^9+7$ 输出即可。

简单来说，就是求：

$$
\sum \prod_{i=1}^m f_{a_i}(m>0,a_1,a_2,\dots,a_m>0,a_1+a_2+\dots +a_m=n)\bmod 10^9+7
$$

## 输入格式

输入的第一行包含一个整数 $n$。

## 输出格式

输出一个整数，为对于 $n$ 的整数 lqp 拆分的权值和 $\bmod 10^9+7$。

## 样例输入

```plain
3
```

## 样例输出

```plain
5
```

## 样例说明

$f_0=0,f_1=1,f_2=1,f_3=2$。

对于 $n=3$，有这样的几种 lqp 拆分：

$3=1+1+1$，权值是 $1\times 1\times 1=1$。

$3=1+2$，权值是 $1\times 1=1$。

$3=2+1$，权值是 $1\times 1=1$。

$3=3$，权值是 $2=2$。

所以答案是 $1+1+1+2=5$。

## 数据规模与约定

$20\%$ 数据满足：$1\leq n\leq 25$.

$50\%$ 数据满足：$1\leq n\leq 10^3$。

$100\%$ 数据满足：$1\leq n\leq 1\times 10^6$。

