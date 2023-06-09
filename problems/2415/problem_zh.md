## 题目描述

Larkin 最近在研究函数的周期点。现在，他想请你帮忙对一类特殊的函数求出其周期点的数目。

所谓周期点是指：对于一个定义域和值域均为 $[0 , m]$ 的函数，如果存在一个 $x \in [0,m]$ 满足 $f^n(x) = x$ ，那么 $x$ 就是这个函数的一个周期点。这里的 $f^n$ 表示函数 $f$ 的迭代，也就是

$$
\begin{aligned}

f^{n} = \overbrace{f \circ \cdots \circ f \circ f}^{n \text{ } f'\text{s}}

\end{aligned}
$$

这里的 $\circ$ 表示函数的合成，例如 $(g \circ h) (x) = g(h(x))$ 。而这一类函数存在以下两点特性：

- 对于任意 $k \in \{ 0 , 1 , \cdots , m \}$ ，$f(k) \in \{ 0 , 1 , \cdots , m \}$ 。
- 对于任意 $k \in \{ 0 , 1 , \cdots , m-1 \}$ ，函数 $f$ 在区间 $[k,k+1]$ 上的图像为直线。也就是说，对于任意 $x\in [k,k+1]$ ，$f(x) = (k+1-x)f(k) + (x-k)f(k+1)$ 。

由于答案很大，所以 Larkin 只要求你求出对于一个给定的整数取余的结果。

![](https://hydro.org.cn/d/bzoj/p/2415/file/pic2.png)

上面两幅图描述的是第三组样例的情况，左图为 $f_3$ ，右图为 $f_3^2$ 。

## 输入格式

**本题有多组测试数据。**

每一组数据的第一行包含一个整数 $m$ 。

接下来的一行描述函数 $f$ 的情况，这一行包含 $m + 1$ 个整数 $f(0),f(1) \cdots f(m)$ ，均介于 $0$ 到 $m$ 之间。

每一组数据的最后一行包含两个整数，$n$ 和用来取余的整数 $mod$ 。

## 输出格式

对于每一组输入数据输出一个答案，表示这个函数的周期点的个数对于 $mod$ 取余的值。如果答案为无穷大则输出 ``Infinity`` 。

```input1
2
2 0 2
2 10
3
0 1 3 2
1 137
3
2 3 0 3
20 10000
```

```output1
4
Infinity
9074
```

## 数据规模与约定

对于 $100 \%$ 的数据，保证 $1 \le m \le 80 , 1 \le n \le 5000 , 1 \le mod \le 10000$ ，数据组数不多于 $10$ 组。

## 题目来源

$\text{swerc2010}$ 。
