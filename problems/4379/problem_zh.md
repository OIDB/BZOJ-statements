


## 题目描述
给定一棵无根树，边权都是1，请去掉一条边并加上一条新边，定义直径为最远的两个点的距离，请输出所有可能的新树的直径的最小值和最大值
## 输入格式
第一行包含一个正整数n(3<=n<=500000)，表示这棵树的点数。
接下来n-1行，每行包含两个正整数u,v(1<=u,v<=n)，表示u与v之间有一条边。
## 输出格式
第一行输出五个正整数k,x1,y1,x2,y2，其中k表示新树直径的最小值，x1,y1表示这种情况下要去掉的边的两端点，x2,y2表示这种情况下要加上的边的两端点。
第二行输出五个正整数k,x1,y1,x2,y2，其中k表示新树直径的最大值，x1,y1表示这种情况下要去掉的边的两端点，x2,y2表示这种情况下要加上的边的两端点。
若有多组最优解，输出任意一组。

```input1
6
1 2
2 3
2 4
4 5
6 5

```
```output1
3 4 2 2 5
5 2 1 1 6
```

## 提示
没有写明提示
## 题目来源
鸣谢Claris


