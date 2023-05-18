


## 题目描述
初始的时候有n个数，第i个数的大小是2^{i-1},我们依次处理每一个数，第i次把第i个数变为编号为i的约数的所有数的异或。比如当n为6的时候：
初始6个数为：
1 2 4 8 16 32
第一次操作1不变所以它们还是：
1 2 4 8 16 32
第二次操作2异或1得到：
1 3 4 8 16 32
第三次操作4异或1得到：
1 3 5 8 16 32
第四次操作8异或3异或1得到：
1 3 5 10 16 32
第五次操作16异或1得到：
1 3 5 10 17 32
第六次操作32异或5异或3异或1得到：
1 3 5 10 17 39
现在我们想知道有多少个正整数b使得可以通过从这最后n个数中取出k个异或起来得到。
 
## 输入格式
第一行三个正整数n，k，p。
 
## 输出格式
一个数输出满足条件的b的数量mod p的值。
 

```input1
3 2 5

```
```output1
3
 
 
```

## 提示
100%的数据n<=109，k<=n，p<=100000
## 题目来源
没有写明来源

