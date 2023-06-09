## 题目描述

有一个字符串生成器，初始时生成的字符串为空串，它每次按照给定概率随机生成一个小写字母，加在当前已生成字符串的后面。

给定 $n$ 个长度为 $l$ 的字符串，每个字符串由小写字母组成。

如果在某个时候，发现每个给定字符串都在当前已生成的字符串中作为子串出现过，生成器就会停下来，将当前生成的字符串作为输出。

求输出字符串长度的期望值。


## 输入格式

第一行包含一个正整数 $c$，表示有 $c$ 组数据。

每组数据的第一行包含三个正整数 $n,l,t$。其中 $t$ 表示生成器仅会生成前 $t$ 个小写字母。  
每组数据的第 $2-(n+1)$ 行，每行包含一个长度为 $l$ 的字符串，每个字符串由前 $t$ 个小写英文字母组成。  
每组数据的第 $n+2$ 行包含 $t$ 个不超过 $10^4$ 的正整数，设第 $i$个正整数为 $x$，那么字符串生成器生成第 $i$ 个小写字母的概率为 $\frac{x}{10^4}$。输入保证这 $t$ 个正整数之和为 $10^4$。


## 输出格式

包含 $c$ 行，依次对应每组数据。每行包含一个实数，表示输出字符串长度的期望值。



```input1
1
2 3 3
aac
abb
3333 3333 3334
```

```output1
40.5060771264
```

## 数据规模与约定

本题共 $10$ 个测试点。

对于 $30\%$ 的数据，$n=1$，$c=1$；  
对于 $60\%$ 的数据，$n\le 4$，$c\le 2$；  

对于 $100\%$ 的数据，$n\le 8$，$c\le 20$，$l\le 6$，$t\le 10$。

其中 $n=1$ 的数据中存在一个测试点，只有你的答案和我们的答案相差小于 $1$ 才为正确，并且这个测试点中 $l=3$，$t=3$；  
对于其他 $9$ 个测试点，只有你的答案和我们的答案相差小于 $0.01$ 才为正确。

**数据保证正确答案不会超过 $5\times 10^6$。**


## 题目来源

`By 佚名提供`

