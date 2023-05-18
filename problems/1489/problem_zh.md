## 题目描述

考虑一个长度为偶数 $n$ 的序列 $a_1, a_2, \dots, a_n$，我们称这个序列为好的，当且仅当存在 $a_1, a_2, \dots, a_n$ 的一个划分 $U=\{ a_{i_1}, a_{i_2}, \dots, a_{i_{n/2}} \}, V=\{ a_{j_1}, a_{j_2}, \dots, a_{j_{n/2}} \}=\{ a_1, a_2, \dots, a_n \}-U$，且 $i_1<i_2< \dots <i_{n/2}, a_{i_1}<a_{i_2}< \dots <a_{i_{n/2}}, j_1<j_2< \dots <j_{n/2}, a_{j_1}<a_{j_2}< \dots <a_{j_{n/2}}$ 比如序列 $3, 1, 4, 5, 8, 7$ 就是一个好的序列。因为它可以分成 $U=\{3, 4, 8\}, V=\{1, 5, 7\}$。而序列 $3, 2, 1, 6, 5, 4$ 则不是一个好的序列。

现在的问题是，针对给出的若干序列，请你判断它们是否是好的序列。

## 输入格式
第一行仅包含一个整数 $m$，表示需要判断 $m$ 个序列。

接下来的 $m$ 行分别给出这些序列。每个序列的输入为一行，每行的第一个数为一个偶数 $n$，表示序列的长度，随后的 $n$ 个整数表示序列本身的元素 $a_1, a_2, \dots, a_n$。同一行的各数之间用一个空格隔开。

## 输出格式
输出 $m$ 行，如果第 $i$ 个序列为好的序列，那么第 $i$ 行输出 `Yes!`，否则输出 `No!`。

```input1
2
6 3 1 4 5 8 7
6 3 2 1 6 5 4
```

```output1
Yes!
No!
```
## 数据范围

对于 $10\%$ 的数据，$n \leq 100$。

对于 $40\%$ 的数据，$n \leq 300$。

对于 $100\%$ 的数据，$1 \leq n \leq 2000$，$1 \le m \leq 25$，$0 \le a_i \le 10^6$。