


## 题目描述
Fibonacci数列是这样一个数列：
F1 = 1， F2 = 1， F3 = 2 . . .
Fi = Fi-1 + Fi-2 (当 i >= 3)
pty忽然对这个古老的数列产生了浓厚的兴趣，他想知道：对于某一个Fibonacci数Fi，
有多少个Fj能够整除Fi (i可以等于j)，他还想知道所有j的平方之和是多少。
## 输入格式
第一行一个整数 **Q,** 表示 **Q** 个询问。
第二行四个整数 **:Q_{1}, A, B, C** 
第 **i** 个询问 **Q_{i} = (Q_{i-1} * A + B) mod C + 1(** 当 **i >= 2)** 
## 输出格式
**Ai** 代表第 **i** 个询问有多少个 **F_{j}** 能够整除 **F_{Qi}** 。
**Bi** 代表第 **i** 个询问所有 **j** 的平方之和。
输出包括两行：
第一行是所有的 **Ai** 之和。
第二行是所有的 **Bi** 之和。
由于答案过大，只需要输出除以 **1000000007** 得到的余数即可。

```input1
2
2  2  1  8

```
```output1
6
55
```

## 提示
对于100%的数据保证：Q <= 3*10^6，C <= 10^7，A <= 10^7，B <= 10^7，1 <= Q1<= C
## 题目来源
没有写明来源

