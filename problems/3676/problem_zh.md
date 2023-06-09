## 题目描述

考虑一个只包含小写拉丁字母的字符串 $s$。我们定义 $s$ 的一个子串 $t$ 的“出现值”为 $t$ 在 $s$ 中的出现次数乘 $t$ 的长度。请你求出 $s$ 的所有回文子串的最大出现值。

## 输入格式

输入只有一行，为一个只包含小写字母（$a\sim z$）的非空字符串 $s$。

## 输出格式

输出一个整数，为逝查回文子串的最大出现值。

```input1
abacaba
```

```output1
7
```

```input2
www
```

```output2
4
```

## 数据规模与约定

数据满足 $1\le |s|\le 300000$，其中 $|s|$ 表示字符串长度。

## 提示

一个串是回文的，当且仅当它从左到右读和从右到左读完全一样。

在第一个样例中，回文子串有 $7$ 个：$\texttt{a},\texttt{b},\texttt{c},\texttt{aba},\texttt{aca},\texttt{bacab},\texttt{abacaba}$，其中：

- $\texttt{a}$ 出现 $4$ 次，其出现值为 $4$：$4\times 1=4$
- $\texttt{b}$ 出现 $2$ 次，其出现值为 $2$：$2\times 1=2$
- $\texttt{c}$ 出现 $1$ 次，其出现值为 $1$：$1\times 1=1$
- $\texttt{aba}$ 出现 $2$次，其出现值为 $6$：$2\times 3=6$
- $\texttt{aca}$ 出现 $1$ 次，其出现值为 $3$：$1\times 3=3$
- $\texttt{bacab}$ 出现 $1$ 次，其出现值为 $5$：$1\times 5=5$
- $\texttt{abacaba}$ 出现 $1$ 次，其出现值为 $7$：$1\times7=7$

故最大回文子串出现值为 $7$。

