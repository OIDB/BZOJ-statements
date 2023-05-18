## 题目描述

你是任意性复杂机器公司（Arbitrarily Complex Machines，ACM）的经理，公司使用更加先进的机械设备生产先进的机器。原来的那一台生产机器已经坏了，所以你要去为公司买一台新的生产机器。你的任务是在转型期内尽可能得到更大的收益。在这段时间内，你要买卖机器，并且当机器被 ACM 公司拥有的时候，操控这些机器以获取利润。因为空间的限制，ACM 公司在任何时候都只能最多拥有一台机器。

在转型期内，有若干台可能卖出的机器。作为先进机器的专家，对于每台机器 $m_i$，你已经知道了其价格 $p_i$ 和可以买入的日期 $d_i$。注意，如果不在第 $d_i$ 天买入机器 $m_i$，那么别的人也会买走这一台机器，也就是说，以后你将没有机会购买这台机器了。如果 ACM 的钱低于一台机器的价格，那么你显然不可能买到这一台机器。

如果你在第 $d_i$ 天买入了机器 $m_i$，那么 ACM 公司可以从第 $d_i+1$ 天开始使用这一台机器。每使用这台机器一天，就可以为公司创造出 $g_i$ 美元的收益。

你可以决定要在买入之后的某一天，以一定的折扣价卖出这一台机器。收购市场对于每一台机器，都有一个折扣价$r_i$。你不能在卖出的那一天使用机器，但是你可以在卖出的那一天再买入一台新的。

在转型期结束后，ACM 公司会卖掉当前所拥有的机器。你的任务就是最大化转型期间 ACM 公司可以得到的收入。

## 输入格式

输入包含若干组测试用例。

每一组测试用例的第一行有三个正整数 $n,c,d$，$n$ 是将会卖出的机器的台数，$c$ 是在转型期开始时公司拥有的美元数量，$d$ 是转型期持续的天数。

之后的 $n$ 行每一行描述了一台机器的情况。

每一行有四个正整数 $d_i,p_i,r_i,g_i$，分别表示这台机器卖出的时间，购买这台机器需要的美元数量，卖出这台机器的折扣价和使用这台机器可以得到的利润。

最后一组测试用例后面的一行由 $3$ 个 `0` 组成，表示输入数据。

## 输出格式

对于每一组测试用例，输出测试用例的编号，之后给出 ACM 公司在第 $d+1$ 天结束后可以得到的最大数量的美元。

请依照下面给出的样例输出。

```input1
6 10 20
6 12 1 3
1 9 1 2
3 2 1 2
8 20 5 4
4 11 7 4
2 10 9 1
0 0 0
```

```output1
Case 1: 44
```

## 数据规模与约定

对于 $100\%$ 的数据，$0\leq n\leq 10^5$，$0\leq c\leq 10^9$，$0\leq d\leq 10^9$，$1\leq d_i\leq d$，$1\leq r_i<p_i\leq 10^9$，$1\leq g_i\leq 10^9$。
