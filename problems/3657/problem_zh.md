


## 题目描述
有n个大于1的正整数a_{1},a_{2},…,a_{n}，我们知道斐波那契数列的递推式是f(i)=f(i-1)+f(i-2)，现在我们修改这个递推式变为f(i)=f(i-1)+f(i-2)+r(i-1)，其中r(x)为a_{1},a_{2},…,a_{n}中为x的约数的个数。现在要求f(m) mod 19940417的值。注：初值f(1)=1,f(2)=1
 
## 输入格式
第一行两个数n,m。
接下来一行n个正整数a_{1},a_{2},…,a_{n}。
 
## 输出格式
输出一行仅一个数，f(m) mod 19940417的值。
 

```input1
3 7
2 2 3


```
```output1
33
 
 
```

## 提示
100%的数据n<=100000,m<=109，2<=ai<=10^9
## 题目来源
没有写明来源

