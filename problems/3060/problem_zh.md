


## 题目描述
给定一个n个点m条边的无向图，问最少删掉多少条边能使得编号小于等于k的点都不在环上。
## 输入格式
       第一行三个整数n，m，k；
       接下来m行每行两个整数a_{i}，b_{i}，表示a_{i}和b_{i}之间有一条无向边。
## 输出格式
 
       一个整数，表示最少的删边数量。

```input1
11 13 5
1 2
1 3
1 5
3 5
2 8
4 11
7 11
6 10
6 9
2 3
8 9
5 9
9 10

```
```output1

3
```

## 提示
数据范围：
       对于100%的数据满足：1 ≤ n ≤ 1,000,000，1 ≤ m ≤ 2,000,000，1 ≤ k ≤ n。
## 题目来源
没有写明来源

