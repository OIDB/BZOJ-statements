## 题目描述
你应该知道，什么是最大公约数：对于任意两个非零整数 $x,y$，若整数 $d$ 能同时被 $x$ 和 $y$ 整除，则称 $d$ 为 $x$ 与 $y$ 的公约数。定义 $x$ 与 $y$ 的最大公约数 $\gcd(x, y)$ 为 $x$ 与 $y$ 的最大的公约数。如 $\gcd(6, 9) = 3$，$\gcd(12, 16) = 4$，$\gcd(25, 32) = 1$，等等。这里，我们定义什么是幸运数：对于一个正整数 $d$，我们使用 $d_i$ 表示 $d$ 在十进制表示下，按从低位到高位顺序的第 $i$ 位数字。设 $F(d)$ 表示 $d$ 的奇数位的数字之和，即 $F(d) = d_1 + d_3 + d_5 + \cdots$；设 $G(d)$ 表示 $d$ 的偶数位的数字之和，即 $G(d) = d_2 + d_4 + d_6 + \cdots$；若 $F(d)$ 与 $G(d)$ 均大于 $0$，且 $F(d)$ 与 $G(d)$ 的最大公约数不超过 $k$，则称 $d$ 为幸运数。其中 $k$ 是一个已知的常数。举个例子来说，若 $d = 641$，则 $d_1 = 1$，$d_2 = 4$，$d_3 = 6$，$F(641) = 1 + 6 = 7$，$G(641) = 4$。此时 $F(d)$ 与 $G(d)$ 的最大公约数即 $\gcd(7, 4)$ 等于 $1$。则当 $k$ 不小于 $1$ 时 $641$ 是幸运数。请你回答下面的问题：对于给定的 $k$，在不小于 $L$ 并且不超过 $R$ 的所有整数中，有多少个数是幸运数？注意，输入文件包含多组测试数据。
## 输入格式
第一行包含一个整数 $T$，表示有 $T$ 组测试数据。
接下来 $T$ 行，每行包含三个整数 $k,l,r$，表示一次询问。
## 输出格式
输出 $T$ 行，每行一个整数，依次表示每组测试数据的答案。
## 样例输入
```plain
5
1 1 10
2 28 34
100 987654321 987654321
1 1 50000
1 50001 100000
```
## 样例输出
```plain
0
5
1
30298
30309
```
## 样例解释
$k = 1$ 时，$1$ 到 $10$ 之间不存在幸运数。

$k = 2$ 时，$28$ 到 $34$ 之间的幸运数有 $28$、$29$、$31$、$32$、$34$，共 $5$ 个。

$k = 100$ 时，$987654321$ 是幸运数。

$k = 1$ 时，$1$ 到 $50000$ 之间的幸运数有 $30298$ 个，$50001$ 到 $100000$ 之间的幸运数有 $30309$ 个。
## 数据范围与约定
对于 $100\%$ 的数据，$1 \le  L \le  R \le  10^{18}$， $1 \le k\le  10^2$，$1 \le T \le 10^3$。