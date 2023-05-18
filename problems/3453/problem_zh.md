## 题目背景
神犇 LYD 虐完 HEOI 之后给傻 X XLk 出了一题：

SHY 是某国的公主，平时的一大爱好是读诗 $\dots$ (中间略) $\dots$ 结果 $\bmod p$ 就可以了
## 题目描述
给定 $k,a,n,d,p$

$f(i)=1^k+2^k+3^k+\dots +i^k$

$g(x)=f(1)+f(2)+f(3)+\dots +f(x)$

求 $(g(a)+g(a+d)+g(a+2d)+......+g(a+nd)) \bmod p$

## 输入格式
有多组数据。

第一行输入数据组数 $T$；

以下 $T$ 行，每行四个整数，代表这组数据中的 $k,a,n,d$。

## 输出格式
共 $T$ 行，每行一个整数，表示计算出的结果。

```input1
5
1 1 1 1
1 1 1 1
1 1 1 1
1 1 1 1
1 1 1 1
```

```output1
5
5
5
5
5
```

## 数据范围
对于 $100\%$ 的数据：$1\leq k\leq 123,0\leq a,n,d\leq 123456789,p=1234567891$

