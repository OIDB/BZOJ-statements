


## 题目描述
Alice和Bob现在在玩的游戏，主角是依次编号为1到n的n枚硬币。每一枚硬币都有两面，我们分别称之为正面和反
面。一开始的时候，有些硬币是正面向上的，有些是反面朝上的。Alice和Bob将轮流对这些硬币进行翻转操作，且
Alice总是先手。具体来说每次玩家可以选择一枚编号为x，要求这枚硬币此刻是反面朝上的。对于编号x来说，我
们总可以将x写成x=c*2^a*3^b，其中a和b是非负整数，c是与2,3都互质的非负整数，然后有两种选择第一种，选择
整数p,q满足a>=p*q,p>=1且1<=q<=MAXQ,然后同时翻转所有编号为c*2^(a-p*j)*3^b的硬币，其中j=0,1,2,..,q。第
二种，选择整数p,q满足b>=p*q,p>=1且1<=q<=MAXQ,然后同时翻转所有编号为c*2^a*3^(b-p*j)的硬币，其中j=0,1,
2,..,q。可以发现这个游戏不能不先进行下去，当某位玩家无法继续操作上述操作时，便输掉了游戏。作为先手的
Alice，总是希望可以在比赛开始之前就知道自己能否获胜。她知道自己和Bob都是充分聪明的，所以在游戏过程中
两人都会最优化自己的策略并尽量保证自己处于不败的情形中
## 输入格式
本题有多组测试数据，第一行输入一个整数T，表示总的数据组数。之后给出T组数据
每组数据第一行输入两个整数n,MAXQ
第二行输入n个整数，第i个数表示第i个硬币的初始状态，0表示反面朝上，1表示正面朝上
对于100%的数据1<=n<=30000,1<=MAXQ<=20,t<=100。
## 输出格式
输出共有t行。对于每一组数据来说，如果Alice先手必胜，则输出"win"（不包括引号），否则输出"lose"

```input1
6
16 14
1 0 0 1 0 0 0 0 1 0 0 0 1 0 1 1
16 14
0 1 0 0 0 1 1 1 1 1 1 0 1 0 0 1
16 11
0 1 0 0 0 1 1 1 0 1 0 0 0 1 0 1
16 12
1 1 1 1 1 1 1 1 0 0 1 1 0 1 1 0
16 4
1 0 0 1 0 0 1 0 0 0 0 1 0 1 1 0
16 20
0 0 0 0 1 0 1 0 0 0 1 0 0 1 0 0

```
```output1
win
lose
win
lose
win
win
```

## 提示
没有写明提示
## 题目来源
By AHdoc命题 鸣谢Loi_DQS上传xiaoyimi提供题面

