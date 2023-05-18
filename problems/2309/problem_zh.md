## 题目描述

对于两个字符串 $a = a_1 a_2 \cdots a_n$ 和 $b = b_1 b_2 \cdots b_n$，定义其最长公共前缀长度 $\text{lcp} (a,b)$ 如下：

$$\text{lcp}(a,b) = \max \{k|0 \le k \le n,k \le m,a_1 a_2 \cdots a_k = b_1 b_2 \cdots b_k \}$$

给定 $n$ 个由小写字母组成的两两不同的非空字符串 $s_1,s_2,\cdots , s_n$，对于一个 $1$ 到 $n$ 的排列 $p=(p_1,p_2,\cdots,p_n)$，定义 $p$ 的价值 $w(p)$ 如下：

$$w(p) = \sum_{i=2}^n (\text{lcp}(s_{p_i-1},s_{p_i}))^2$$

我们设能够产生最大价值的排列为 $p^ * _g$。此外，还有 $q$ 个附加任务。对于第 $i$ 个任务，给定两个 $1$ 到 $n$ 之间的不同的整数 $x_i$ 和 $y_i$。对于排列 $p$，若 $p$ 在满足 $w(p) = w(p^*_g)$ 的前提条件之下，同时满足第 $x_i$ 个字符串 $s_{x_i}$ 恰好排在第 $y_i$ 个字符串 $s_{y_i}$ 之前，即 $\text{pos}(s_{x_i}) + 1 = \text{pos}(s_{y_i})$，其中 $\text{pos}(s_i)$ 表示字符串 $s_i$ 在排列中的位置，则排列 $p$ 还将获得 $2^i$ 的奖励。所有任务的奖励之和称之为总任务奖励。我们设能够使得总任务奖励最大的排列为 $p^*_b$。试求：

1. $w(p^*_g)$，即可能产生的最大价值；
2. $p^*_b$，在保证最大价值前提下，可以使总任务奖励最大的排列。

## 输入格式

第一行包含两个整数 $n$ 和 $q$，表示字符串和附加任务的数量，中
间用一个空格隔开。\
接下来 $n$ 行，描述字符串，其中第 $i$ 行包含一个字符串 $s_i$。\
接下来 $q$ 行，描述附加任务，其中第 $i$ 行包含两个整数 $x_i$ 和 $y_i$，中间用一个空格隔开。

## 输出格式

输出是第一行最大价值；\
第二行若干个数，每两个数之间用一个空格隔开，这一行第一个数表示满足附加任务的数量 $k$，接下来 $k$ 个数为这些任务的序号，序号从 $1$ 开始，按从小到大的顺序输出； \
第三行包含 $n$ 个用一个空格隔开的正整数，表示一个 $1$ 到 $n$ 的排列 $p^*_b$。

```input1
4 6
a
b
abc
bc
1 2
1 3
3 1
4 2
2 4
2 4
```
```output1
2
4 1 3 5 6
3 1 2 4
```

## 数据规模与约定

对于 $10\%$ 的数据，$n \le 10$，$q=1$，每个字符串的长度不超过 $50$；\
对于 $20\%$ 的数据，$n \le 50$，$q=1$，每个字符串的长度不超过 $50$；\
对于 $50\%$ 的数据，$n,q \le 1000$，每个字符串的长度不超过 $1000$；\
对于 $70\%$ 的数据，任意字符串不为其他任何一个字符串的前缀；\
对于 $100\%$ 的数据，$n \le 4 \times 10^4$，$q \le 10^5$，每个字符串的长度不超过 $10^4$，所有字符串的长度和不超过 $2 \times 10^5$。

## 评分方式

对于一个测试点： 
- 如果输出文件的第一行正确可以得到 $2$ 分；
- 如果输出文件的第二行正确可以得到 $4$ 分；
- 如果输出文件的第三行正确可以得到 $4$ 分；
- 如果输出文件的三行都正确则可以得到 $10$ 分。 
- 对于第三问中的排列，如果存在多个解， 则输出任意一个解均可得分。 若某问无法完成，也请按照格式输出，以避免测评失败。

## 题目来源

鸣谢 wjbzbmr