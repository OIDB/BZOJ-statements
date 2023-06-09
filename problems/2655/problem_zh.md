## 题目描述

一个序列 $a_1,\dots,a_n$ 是合法的，当且仅当：
长度为给定的 $n$。$a_1,\dots,a_n$ 都是 $[1,A]$ 中的整数。$a_1,\dots,a_n$ 互不相等。一个序列的值定义为它里面所有数的乘积，即 $\prod\limits_{i=1}^{n}a_i$。

求所有不同合法序列的值的和。两个序列不同当且仅当他们任意一位不一样。输出答案对一个数 $mod$ 取余的结果。

## 输入格式

一行 $3$ 个数，$A，n，mod$。意义为上面所说的。

## 输出格式

一行结果。

## 样例

```input1
9 7 10007
```

```output1
3611
```

## 数据规模和约定

对于 $5\%$ 的数据 $A,n\le10$。

对于 $20\%$ 的数据 $A\le 10^3,n\le 20$。

对于 $50\%$ 的数据 $A\le 10^9,n\le 20$。

对于 $100\%$ 的数据 $A\le 10^9,n\le 500$，$mod \le 10^9$ 且为素数，$mod > A>n+1$。

