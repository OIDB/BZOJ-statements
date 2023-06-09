## 题目描述

给你一个由 `A`,`G`,`T`,`C` 组成的字符串，其实就是基因串。

大家知道基因串是 $\text{AGTCAGTCAGTC}$ 这样的形式。现在对这个字符串进行位置编号，从 $0$ 开始，到 $n-1$，$n$ 代表整个字符串的长度。现在给出 $t$ 个要求，希望你对给出的字符串进行一些变动，变动的方式有三种：

1. 设置某个位置的字符不可变；

2. 将某个位置的字符上升一个，例如从 $\text{C}$ 变成 $\text{A}$；

3. 将某个位置的字符下降一个，例如从 $\text{T}$ 变成 $\text{G}$。

**注意两个相邻位置的字符不能同时发生变动**。

对于这 $t$ 个要求，它们分别会给出一些位置，要求从这些位置取出来的字符形成一个回文串。

## 输入格式

**本题有多组数据**

第一行给出 $n,t$。

第二行输入所给字符串。

接下来有 $t$ 行，每行先给出一个长度 $l$ ，再给出 $l$ 个数字其值在 $[0，n-1]$。

## 输出格式

输出 `YES` 或者 `NO`。

```input1
5 3
AGTAT
2:1 4
2:0 1
3:0 2 4
5 3
CATGC
0:
2:0 3
2:3 4
00
```

```output1
YES
NO
```

## 数据规模与约定

$100\%$ 的数据满足：$1 \le n \le 1 \times 10^5$，$1 \le t \le 6 \times 10^3$。