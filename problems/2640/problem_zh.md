

## 题目描述
在平面直角坐标系中有 $N$ 条互不相交(没有公共点)且所在直线不会经过 $(0,0)$ 的线段。有一个人站在 $(0,0)$，他的视野是 360 度的。但是他在某一个方向上的视野会被该方向上碰到的第一条线段所阻挡，问他能看到的区域面积有多大（数据保证是有限面积）。如下图（样例），可以看到的面积就是 11。  

![pic1](file://pic1.jpg)

为了加大难度，他想知道，在删除一条线段的情况下能看到最大多大的面积（不保证是有限面积）。  
进一步，他还想知道，在删除两条线段的情况下能看到最大多大的面积（不保证是有限面积）。  

## 输入格式

第一行一个整数 $N$ 表示线段条数。  
接下来 $N$ 行，每行四个整数 $x_1,y_1,x_2,y_2$ 表示一条线段两个端点的坐标。

## 输出格式
第一行一个**保留两位小数**的实数，表示可见区域的面积。  
第二行两种可能，如果删除一条线段以后能使得看到的区域有无限大输出 `infinite`，否则输出一个**保留两位小数**的实数，表示这种情况下能看到的最大面积。  
第三行两种可能，如果删除两条线段以后能使得看到的区域有无限大输出 `infinite`，否则输出一个**保留两位小数**的实数，表示这种情况下能看到的最大面积。

```input1
6
-1 -1 0 -1
0 -2 1 -1
-1 1 0 2
0 1 1 1
2 -2 2 2
-2 -2 -2 2

```

```output1
11.00
infinite
infinite
```

## 数据规模和约定

对于 $100\%$ 数据，$1\leq n \leq 50000$，坐标的绝对值 $\leq 10^3$。

## 题目来源
没有写明来源
