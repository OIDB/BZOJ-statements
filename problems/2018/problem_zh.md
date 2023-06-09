## 题目描述

农夫约翰有 $3n$ 头牛，编号依次为 $1 \ldots 3n$，每头牛都有一个整数值的体重 $w$；约翰准备参加农场技艺大赛，向广大的农业社区展示他的奶牛。

大赛规则允许约翰带 $n$ 头牛参赛. 约翰给每头牛赋予了一个「有用度」$u_i$，它表示了某头牛在比赛中的有用程度. 约翰希望他选出的奶牛的有用度之和最大。

有可能选出很多组的 $n$ 头牛都能达到有用度最大和. 约翰害怕选出的 $n$ 头牛的总重量会给大赛带来震撼，所以，要考虑优先选择体重轻的奶牛。

帮助约翰选出 $n$ 头总重量最轻，并且有用度之和最大的奶牛. 输出体重模 $m$ 后的余数。

注意：为了使输入更快，约翰使用了一个多项式来生成每头牛的体重和有用度，对每头牛 $i$，体重和有用度的计算公式为：

$$
w_i= \ (ai^5+bi^2+c) \bmod\ d
$$

$$
u_i=\ (ei^5+fi^3+g) \bmod\ h
$$

这个多项式有时会生成重复的数，你的程序要正确处理这种情况。

## 输入格式

第一行：$10$ 个空格分开的整数：$n, a, b, c, d, e, f, g, h, m$。

## 输出格式

第一行：满足总重量最轻，且用度之和最大的 $n$ 头奶牛的总体重模 $m$ 后的余数。

```input1
2 0 1 5 55555555 0 1 0 55555555 55555555
```
```output1
51
```

## 样例说明 1

公式生成的体重和有用度分别为：体重：$5, 6, 9, 14, 21, 30$ 有用度：$0, 1, 8, 27, 64, 125$。

## 数据规模与约定

对于 $100\%$ 的数据，$1 <n< 5\times10^5$，$1<w \leq d$，$1 <u_i<h$，$10^7< m <10^9$，$0<a,b,c,d,e,f,g,h<10^9$。

## 题目来源

Silver