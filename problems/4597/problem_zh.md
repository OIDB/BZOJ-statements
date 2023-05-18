


## 题目描述
你的面前有N个数排成一行。分别为A1, A2, … , An。你打算在每相邻的两个 Ai和 Ai+1 间都插入一个加号或者
减号或者乘号。那么一共有 3^(n-1) 种可能的表达式。你对所有可能的表达式的值的和非常感兴趣。但这毕竟太
简单了，所以你还打算支持一个修改操作，可以修改某个Ai 的值。你能够编写一个程序对每个修改都输出修改完
之后所有可能表达式的和吗？注意，修改是永久的，也就是说每次修改都是在上一次修改的基础上进行， 而不是
在最初的表达式上进行。
## 输入格式
第一行包含 2 个正整数 N 和 Q，为数的个数和询问的个数。
接下来一行 n 个非负整数，依次表示a1,a2...an
在接下来 Q 行，其中第 ?? 行两个非负整数Ti 和Vi，表示要将 A_{ti} 修改为 Vi。其中 1 ≤ Ti ≤ N。
保证对于 1 ≤ J ≤ N, 1 ≤ i≤ Q，都有 Aj,Vi ≤ 10^4。
N,Q<=100000,本题仅有三组数据
## 输出格式
输出共 Q 行，其中第 i 行表示第 i 个询问之后所有可能表达式的和，对10^9 + 7 取模。

```input1
5 5
9384 887 2778 6916 7794
2 8336
5 493
3 1422
1 28
4 60

```
```output1
890543652
252923708
942282590
228728040
608998099
```

## 提示
没有写明提示
## 题目来源
By 佚名上传

