

## 题目描述

某个房子的屋顶如下图所示。

 ![](file://pic1.jpg)
 
在单位时间单位长度降雨量为 $1$ 单位的时候，每条“屋顶”，都有一个单位时间落下的水量（就是单位时间从屋顶较低的那一侧落下去的水量）。

现在希望对于每个屋顶，算出它的落水量。 

## 输入格式

第一行一个正整数 $n$，表示屋顶的个数。 

接下来 $n$ 行，每行 $4$ 个 $[-10^6,10^6]$ 内的整数 $x_0,x_1,y_0,y_1$，描述一个屋顶的两个端点坐标，保证屋顶一定是斜的且没有任何公共点。 

## 输出格式

共 $n$ 行，每行一个非负整数，第 $i$ 行的非负整数表示第 $i$ 个屋顶的落水量。 

```input1
6
13 7 15 6
3 8 7 7
1 7 5 6
5 5 9 3 
6 3 8 2
9 6 12 8

```
```output1
2
4
2
11
0
3
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n\le2\times10^4$。