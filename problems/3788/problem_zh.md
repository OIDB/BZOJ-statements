## 题目描述

话说考古学家 ZL 走进了一个山洞……

ZL 在山洞深处发现了一组密码锁，并断定这里藏着数不清的宝藏。经过一番寻找，ZL 发现该密码锁上写着一串阿拉伯数字，看起来这些数字中有着一些微妙的联系。于是他动用了 $120$ 分脑细胞，凭着藐视一切 IMO 选手的强大逻辑推理能力，找到了规律，并破解了几个密码锁。

可 ZL 毕竟是人，他也是会累的呀 T_T。

况且他的 GPS 显示前方还有成百上千个密码锁！！！！

于是他把问题简化了一下，求助于身为 OI 神犇的你。

数列 $a_n$ 由如下关系式定义：

1. $a[0]=0$；
2. $a[n]=f(a[n-1])$。

其中 $f(x)$ 是一个正整数系数的 $m$ 次多项式。

对任意给定的 $x$ 和 $y$，求 $a_x$ 和 $a_y$ 的最大公约数 $d$。

令 $s$ 为 $d$ 模 $x$ 的余数，$t$ 为 $d$ 模 $y$ 的余数。

给定 $r$ 和一个奇质数 $p$，保证 $r$ 不是 $p$ 的整数倍。

废话完毕，现在我们的问题是：

求方程 $(rx^2+sx+t) \bmod p=0$ 有几个模 $p$ 意义下的正整数解。

对每个函数 $y=f(x)$ 将进行 $T$ 次询问。

## 输入格式

输入文件包括 $T+3$ 行。

第一行一个正整数 $m$。

第二行 $m+1$ 个正整数 $c_m \dots c_0$，其中$c_i~(m \ge i \ge 0)$ 表示 $f(x)$ 中 $x_i$ 的系数。

第三行一个正整数 $T$，表示询问次数。

以下 $T$ 行每行四个正整数，分别表示 $x,y,r,p$。

## 输出格式

输出文件包含 $T$ 行，每行仅输出一个整数表示方程有多少组解（模 $p$ 的意义下）。

```input1
1
2 1
1
4 8 7 3
```

```output1
0
```

## 数据规模与约定

对于 $100\%$ 的数据，$T \le 10^3$，$m \le 10$，$x<y$，$x \le 10^5$，$y \le 10^8$，$p \le 10^8$。
