## 题目描述

今天是贝茜的生日，为了庆祝自己的生日，贝茜邀你来玩一个游戏． 贝茜让 $n$ 头奶牛坐成一个圈．除了 $1$ 号与 $n$ 号奶牛外，$i$ 号奶牛与 $i - 1$ 号和 $i + 1$ 号奶牛相邻。$n$ 号奶牛与 $1$ 号奶牛相邻。农夫约翰用很多纸条装满了一个桶，每一张包含了一个独一无二的 $1$ 到 $10^6$ 的数字。接着每一头奶牛 $i$ 从柄中取出一张纸条 $a_{i}$ 。每头奶牛轮流走上一圈，同时拍打所有编号能整除在纸条上的数字的牛的头，然后做回到原来的位置。牛们希望你帮助他们确定，每一头奶牛需要拍打的牛。

## 输入格式

第 $1$ 行包含一个整数 $n$，接下来第 $2$ 到 $n + 1$ 行每行包含一个整数 $a_{i}$。

## 输出格式

第 $1$ 到 $n$ 行，每行的输出表示第 $i$ 头奶牛要拍打的牛数量。

## 样例

```input1
5 
2
1
2
3
4
```

```output1
2
0
2
1
3
```



## 数据规模与约定

对于 $100\%$ 的数据，$1 \leq n \leq 100000$ 。

## 题目来源

Silver