


## 题目描述
小Y来到了一个新的城市旅行。她发现了这个城市的布局是网格状的，也就是有n条从东到西的道路和m条从南到北
的道路，这些道路两两相交形成n×m个路口 (i,j)(1≤i≤n,1≤j≤m)。她发现不同的道路路况不同，所以通过不
同的路口需要不同的时间。通过调查发现，从路口(i,j)到路口(i,j+1)需要时间 r(i,j)，从路口(i,j)到路口(i+1
,j)需要时间c(i,j)。注意这里的道路是双向的。小Y有q个询问，她想知道从路口(x1,y1)到路口(x2,y2)最少需要
花多少时间。
## 输入格式
第一行包含 2 个正整数n,m，表示城市的大小。
接下来n行，每行包含m?1个整数，第i行第j个正整数表示从一个路口到另一个路口的时间r(i,j)。
接下来n?1行，每行包含m个整数，第i行第j个正整数表示从一个路口到另一个路口的时间c(i,j)。
接下来一行，包含1个正整数q，表示小Y的询问个数。
接下来q行，每行包含4个正整数 x1,y1,x2,y2，表示两个路口的位置。
## 输出格式
输出共q行，每行包含一个整数表示从一个路口到另一个路口最少需要花的时间。

```input1
2 2
2
3
6 4
2
1 1 2 2
1 2 2 1

```

```output1
6
7
```

## 提示
 题解:[JudgeOnline/upload/201603/4456 sol.txt](/JudgeOnline/upload/201603/4456 sol.txt)
## 题目来源
没有写明来源


