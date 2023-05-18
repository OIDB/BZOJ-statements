## 题目描述

J 国有 $n$ 个大城市，城市之间建立了发达的高速路网。在 J 国，两个城市之间的高速公路都是直线连接的，且没有两条高速公路在端点城市以外的地方相交。另外，J 国已经做好了战争规划，使得在任意一个城市或任意一个道路被摧毁的情况下，整个国家的路网依然能够畅通。

K 国打算闪电突击 J 国，他们储备了大量的 ICBM（Intercontinental Ballistic Missile，洲际弹道导弹），一枚导弹能够摧毁 J 国的一个城市。为了让闪击更有战略意义，K 国的战争领导层提出了L个方案，每个方案是一个序列 $(a_1,a_2,\dots,a_n)$，保证 $a_1-a_2,a_2-a_3,\dots,a_{n-1}-a_n,a_n-a_1$ 之间都有高速公路连接，且没有一个城市在序列上重复出现。这个方案的实施方法就是部署 ICBM 摧毁序列表示的环内所有的城市（包括落在环上的）。

现在战争领导层打算统计每个方案的导弹消耗。这个任务就交给你了。

## 输入格式

第一行两个数 $n,m$，表示 J 国的城市数量以及高速路数量。  
接下来 $m$ 行，每行两个数 $x,y$，表示 $x$ 和 $y$ 之间有一条高速路连接。保证没有重边和自环。  
接下来 $n$ 行，每行两个整数 $X_i,Y_i$，表示第 $i$ 个城市的平面坐标。  
接下来一行 $L$，表示方案个数。  
接下来 $L$ 行，每行以一个数 $k$ 开头，接下来 $k$ 个数$a_1,a_2,a_3,\dots,a_k$，表示一个方案。


## 输出格式

$L$ 行，每行一个数，表示对应方案需要的导弹数量。

```input1
5 8
5 1
5 2
5 3
5 4
4 1
1 2
3 2
3 4
0 0
2 0
2 2
0 2
1 1
1
4 4 3 2 1
```

```output1
5
```

## 数据规模与约定

对于 $100\%$ 的数据，$n \le 33333$，$L \le 3 \times 10^3$，$k \ge 3$，$S \le 10^5$，$|X_i|,|Y_i| \le 10^9$。
