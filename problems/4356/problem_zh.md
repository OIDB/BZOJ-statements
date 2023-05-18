

## 题目描述
给出一个 $n\times m$ 的网格图，有一些方格里面存在城市，其中首都位于网格图的左上角。

你可以沿着网络的边界走，要求你走的路线是一个环并且所有城市都要被你走出来的环圈起来。即想从方格图的外面走到任意一个城市一定要和你走的路线相交。

你沿着方格的边界走是需要费用的，不同的边界费用可能不同，求最小代价。
## 输入格式
第一行两个整数 $n,m$，表示网格的长和宽。
## 输出格式

一行一个整数，表示最小代价。

```input1
3 3
1 0 0
1 0 0
0 0 1
1 4 9 4
1 6 6 6
1 2 2 9
1 1 1
4 4 4
2 4 2
6 6 6
```
```output1
38
```
```input2
3 3
1 0 1
0 0 0
0 1 0
2 1 1 3
5 6 1 1
2 1 1 3
2 1 1
3 4 1
4 1 1
5 1 2
```
```output2
22
```

## 提示
对于 $100\%$ 的数据，$1\le n,m\le 400$，走过边界的代价为正整数且不超过 $10^9$。
## 题目来源
没有写明来源  