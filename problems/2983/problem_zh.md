

## 题目描述
定义任意两小写字母间有一个差别值 $X$，假设 $26$ 个小写字母随意排列构成的都是单词，则对于一个单词可算出差别总和为 $\rm sum$，例如：假设 $X[{\tt e}-{\tt l}]=3$，$X[{\tt l}-{\tt y}]=2$，$X[{\tt l}-{\tt l}]=1$，则单词 $\tt elly$ 的 $\rm sum$ 值为 $3+1+2=6$。
现在给出 $n$ 和 $m$，$n$ 表示 $\rm sum$ 值的上限（可以等于 $n$），$m$ 表示已知关系个数，接下来 $m$ 行，每行三个数 $L_1$，$L_2$，$f$，表示字母 $L_1$ 到 $L_2$ 和 $L_2$ 到 $L_1$ 的 $X$ 值都为 $f$，若未提及的字母对则默认它们的 $X$ 值为 $1$，则问总共可形成多少符合条件的单词？
 
## 输入格式
第一行 $n,m$。

之后 $m$ 行，每行三个数 $L_1$，$L_2$，$f$，保证每对字母最多出现一次。
 
## 输出格式
 
符合条件的单词总数 $\mod 1000 000 007 $ 的结果。
 

```input1
20 10
e l 3
e o 1
o n 2
o r 4
r a 4
i n 5
e n 2
n t 3
t w 3
w i 5


```
```output1
 470059518
```

## 数据规模与约定

对于 $50 \%$ 的数据，$1 \leq n \leq 1 \times 1 \times 10^8$。

对于 $100 \%$ 的数据，$1 \leq X \leq 5$，$1 \leq f \leq 5$，$1 \leq n \leq 1 \times 1 \times 10^{12}$