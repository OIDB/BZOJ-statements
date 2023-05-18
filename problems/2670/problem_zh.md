


## 题目描述
    
定义n个数X1,X2,...Xn(n>1)的几乎平均数为ΣXi/(n-1)
对于给出的长度为N的一个序列S，要求回答Q个询问
每个询问会给出L,R(1<=L<R<=N)，请找出a与b(L<=a<b<=R)使得Sa,Sa+1,Sa+2,...Sb的几乎平均数最大
## 输入格式
第一行两个正整数N,Q
第二行N个数表示序列S
接下来Q行，每行两个数L,R
## 输出格式
**　对于每个询问回答一行，用一个既约分数表示最大的几乎平均数
若答案为整数x，输出x/1
** 

```input1
3 2
-2 -1 -2
1 2
1 3

```
```output1
-3/1
-5/2
```

## 提示
数据规模和约定
对于所有数据|Si|<=10^6
TEST N Q TEST N Q 
1 =10 =10 11 =3*10^4 =10^4 
2 =100 =100 12 =4*10^4 =10^4 
3 =1000 =1000 13 =5*10^4 =10^4 
4 =2000 =2000 14 =6*10^4 =2*10^4 
5 =5000 =5000 15 =7*10^4 =2*10^4 
6 =10^4 =5000 16 =8*10^4 =3*10^4 
7 =10^4 =10^4 17 =9*10^4 =3*10^4 
8 =2*10^4 =5000 18 =10^5 =10 
9 =2*10^4 =10^4 19 =10^5 =3*10^4 
10 =3*10^4 =5000 20 =10^5 =3*10^4
 
 
 
 
 
## 题目来源
没有写明来源

