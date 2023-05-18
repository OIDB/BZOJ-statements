## 题目描述

给你 $n$ 颗宝石，每颗宝石都有重量和价值。要你从这些宝石中选取一些宝石，保证总重量不超过 $w$，且总价值最大为，并输出最大的总价值。

## 输入格式

输入文件中包含多组数据。每组数据的格式如下：

第一行是两个正整数 $n$ 和 $w$，分别表示宝石的数目和最多能带走的宝石重量。

接下来的 $n$ 行，每行有两个正整数 $weight_i$ 和 $value_i$，分别表示第 $i$ 颗宝石的重量和价值，同一行的两个正整数之间用空格隔开。

最后一组数据的后面有两个 `-1`，表示文件的结束。这两个 `-1` 并不代表一组数据，你不需对这组数据输出结果。

## 输出格式

对于输入的每组数据，输出一个整数从 $c$，表示小 P 最多能带走的宝石的总价值。每个结果整数 $c$ 单独占一行。


```input1
4 10
8 9
5 8
4 6
2 5
4 13
8 9
5 8
4 6
2 5
16 75594681
393216 5533
2 77
32768 467
29360128 407840
112 68
24576 372
768 60
33554432 466099
16384 318
33554432 466090
2048 111
24576 350
9216 216
12582912 174768
16384 295
1024 76
-1 -1

```

```output1
14
19
1050650
```
## 数据规模与约定

对于 $100\%$ 的数据：

- 输入文件中数据的组数不超过 $20$；
- $n \le 100$，$w\le 2^{30}$；
- $1\le weight_i\le 2^{30}$， $0\le value_i\le 2^{30}$；
- 保证 $weight_i$ 能写成 $a\times 2^b$ 的形式（$1\le a\le 10$，$0\le b\le 30$）；
- 保证 $c$ 不会超过 $2^{30}$。