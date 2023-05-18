## 题目描述

小T最近在学着买股票，他得到内部消息：F 公司的股票将会疯涨。股票每天的价格已知是正整数，并且由于客观上的原因，最多只能为 $n$ 。在疯涨的 $k$ 天中小 T 观察到：除第一天外每天的股价都比前一天高，且高出的价格（即当天的股价与前一天的股价之差）不会超过$m$，$m$ 为正整数。并且这些参数满足 $m(k-1)<n$。小 T 忘记了这 $k$ 天每天的具体股价了，他现在想知道这 $k$ 天的股价有多少种可能。

## 输入格式

只有一行用空格隔开的四个数：$n,k,m,p$。

## 输出格式

仅包含一个数，表示这 $k$ 天的股价的可能种数对于 $p$ 的模值。



```input1
7 3 2 997
```



```output1
16
```

## 样例说明

输出样例的 16 表示输入样例的股价有 16 种可能：
`{1，2，3}， {1，2，4}， {1，3，4}， {1，3，5}， {2，3，4}， {2，3，5}， {2，4，5}， {2，4，6}， {3，4，5}， {3，4，6}， {3，5，6}， {3，5，7}， {4，5，6}， {4，5，7}， {4，6，7}， {5，6，7}`

## 数据规模与约定

对于 $20\%$ 的数据 $m,n,k,p\le 2 \times 10^4$。

对于 $100\%$ 的数据 $ m,k,p\le 10^9 $，$ n \le 10^{18}$。
