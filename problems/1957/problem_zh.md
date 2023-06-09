**题面不完整。**

## 题目描述

Infinite City 是无限的坐标形式城市，每个整点都是十字路口。

Bears 试图袭击位于 $(0,0)$ 的蜂蜜仓库，乘汽车从点 $A$ 出发。州长试图通过封锁道路，尽可能让汽车远离仓库。汽车每到一个路口，州长会封锁四个方向中的一个，汽车选择未封锁道路行驶一个单位；存在一些主要道路，不能封锁，双方都选择最优方案，求最后汽车行驶过程中 $D$ 值最小值。对坐标 $(x,y)$，$D = \max(|x|,|y|)$。
<!--
----

洛谷题面：

给定 $N$ 条长度为 $1$ 的线段，定义他们为「标记线」。

现在在点 $(A,B)$ 处有一个强盗，他要前往 $(0,0)$，警察们可以任意选择一个点，关闭他四周的任意一条线段。比如选择点 $(0,0)$，线段 $(-1,1) \to (1,1)$，$(-1,1)\to (-1,-1)$，$(-1,-1) \to (1,-1)$，$(1,-1) \to (1,1)$ 其中之一将会被关闭，但是关闭的线段中不能有与标记线 **直接相连** 的线段。比如 $(0,0) \to (0,2)$ 与 $(0,1) \to (0,3)$ 是直接相连的，但是 $(-1,1) \to (1,1)$ 与 $(0,0) \to (0,3)$ 不是。

强盗可以到达关闭的线段上的点，但是不能通过关闭的线段离开。 求强盗离 $(0,0)$ 的最近的距离的最大值 $D$。

本题中的 $(a,b) \to (c,d)$ 代表一条从 $(a,b)$ 连向 $(c,d)$ 的线段。

## 输入格式

第一行两个整数 $A,B$ 代表强盗初始在 $(A,B)$。 第二行一个整数 $N$ 代表标记线数。 接下来 $N$ 行每行两个整数 $X_1,Y_1,X_2,Y_2$ 代表一条标记线 $(X_1,Y_1) \to (X_2,Y_2)$。

## 输出格式

一行一个整数代表强盗离 $(0,0)$ 的最近的距离的最大值 $D$。-->


```input1
70 -64
0
```

```output1
70
```
<!--
## 样例说明 1

样例说明 1 对于样例 $1$，如下图所示： ![](https://cdn.luogu.com.cn/upload/image_hosting/cqukdqmc.png) 选择的点为 $(0,0)$，关闭的线段为 $(1,1) \to (1,-1)$。 

## 数据规模与约定

对于 $100\%$ 的数据，$|A|,|B|,|X_1|,|Y_1|,|X_2|,|Y_2| \le 10^6$，$0 \le N \le 500$，保证每条标记线 $X_1=X_2$ 或者 $Y_1=Y_2$。-->


## 题目来源

BZOJ 原题面缺失，可以前往 [洛谷 P6761](https://www.luogu.com.cn/problem/P6761) 查看另一个版本的中文题面或查看 [英文原版题面](https://boi.cses.fi/files/boi2010_day1.pdf)。