## 题目描述

Blinker 有非常多的仰慕者，他给每个仰慕者一个正整数编号。

而且这些编号还隐藏着特殊的意义，即编号的各位数字之积表示这名仰慕者对 Blinker 的重要度。

现在 Blinker 想知道编号介于某两个值 $a,b$ 之间，且重要度为某定值 $k$ 的仰慕者编号和。

多组询问。

## 输入格式

输入的第一行是一个整数 $n$，表示询问数。  
接下来 $n$ 行，每行三个整数 $a,b,k$，表示一个询问。

## 输出格式

输出 $n$ 行，每行表示一个询问的答案。

答案对 $20120427$ 取模。

```input1
3 
1 14 4 
1 30 4 
10 60 5 
```

```output1
18 
40 
66 
```

## 数据规模与约定

对于 $20\%$ 的数据，保证： $2\leq a\leq b\leq 10^9$，$1\leq n\leq 30$。  
对于 $50\%$ 的数据，保证：$2\leq a\leq b\leq 10^{18}$，$1\leq n\leq 30$。  
对于 $100\%$的数据，保证： $2\leq a\leq b\leq 10^{18}$，$1\leq n\leq 5\times 10^3$。