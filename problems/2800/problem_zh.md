## 题目描述

给出n个整数 $X_1,X_2,...X_n$，再给出两个正整数$a$、$b$，可以进行下面四种操作：

1. 选择正整数$l,r$ ($1 \le l \le r \le n$），将$X_l,X_{l+1},...,X_r$都加上$a$。
2. 选择正整数$l,r$ （$1 \le l \le r \le n$），将$X_l,X_{l+1},...,X_r$都减去$a$。
3. 选择正整数$l,r$ （$1 \le l \le r \le n$），将$X_l,X_{l+1},...,X_r$都加上$b$。
4. 选择正整数$l,r$ （$1 \le l \le r \le n$），将$X_l,X_{l+1},...,X_r$都减去$b$。
   求最少的操作次数将${X_i}$全部变成$0$。

## 输入格式

第一行三个正整数$n$,$a$,$b$。
第二行$n$个整数，依次表示$X_1,X_2,...X_n $。

## 输出格式

一个正整数，表示最少的操作次数。如果不存在方案，输出$-1$。

## 输入样例

```input1
5 2 3
1 2 1 1 -1
```

## 输出样例

```output
5
```
