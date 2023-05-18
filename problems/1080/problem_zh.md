## 题目描述

一个编码方案把每个字符对应到一个 01 串。例如 $\text{\{1,1010,01,10101\}}$ 就是一个编码方案，它把四个字符（假设
它们为 $a,b,c,d$）分别对应到串 $\text{1}$、$\text{1010}$，$\text{01}$，$\text{10101}$。字符串的编码为各字符编码的连接。例如，在刚才的编码方案中，字符串 $\text{cac}$ 的编码为 $\text{01101}$，$\text{dcb}$ 的编码为 $\text{10101011010}$。进一步分析发现，刚才的编码是相当劣质的，因为字符串 $\text{ba}$，$\text{acc}$ 和 $\text{d}$ 的编码都是 $\text{10101}$。对于一个编码方案，你的任务是找出三个不同的字符串，使得它们的编码全相同。换句话说，找一个 01 编码串，使得它至少有三种解码方式。如果有多组解，这个编码串应当尽量短。

## 输入格式

第一行包含一个整数 $n$，即符号的个数。以下 $n$ 行每行为一个长度不超过 $50$ 的 01 串（可能为空串），即各符号的编码。

## 输出格式

仅一行，包含一个整数，即最短编码的长度。如果无解，输出 `-1`。

```input1
4
1
1010
01
10101
```

```output1
5
```

## 数据规模与约定

对于 $100\%$ 的数据，$2\le n\le 30$。

