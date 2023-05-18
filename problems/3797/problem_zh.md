## 题目描述

外星人制造了超级电脑来思考生命，宇宙，以及世界万物的答案，最后得出了 `42` 这个结果。人们并不满意于这个答案，于是再一次设计了超级电脑。经历了 $π$ 百万年的计算，再一次得出了新的答案。

答案是由一些字符串组成的，每个字符串都只包含 `(` 和 `)` 两种字符。

现在的问题是，从这些字符串中选取一些，按照一定的顺序连接起来，使得构成一个合法的括号序列而且长度尽量长。

## 输入格式

本题存在多组数据，请执行到文件底结束，任两组数据间存在一空行。

第一行正整数 $n$ 表示字符串个数。

接下来 $n$ 行每行一个字符串（编号从 $1$ 到 $n$）。

## 输出格式

对于每组数据输出最大长度。

```input1
3
()
(()
)
```

```output1
6
```

## 样例解释

最长的字符串为 `(())()`。

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 10^3$，字符串的总长度不超过 $10^4$。
