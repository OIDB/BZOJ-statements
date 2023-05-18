## 题目描述

作为水污染管理部门的一名雇员，你需要监控那些被有意无意倒入河流、湖泊和海洋的污染物。你的其中一项工作就是估计污染物对不同的水生态系统（珊瑚礁、产卵地等等）造成的影响。

![](file://pic1.jpg)

你计算所使用的模型已经在图 $1$ 中被说明。海岸线（图 $1$ 中的水平直线）为 $x$ 轴，污染源位于原点 $(0, 0)$。污染的蔓延呈半圆形，多边形代表了被波及的生态系统。你需要计算出生态系统被污染的面积，也就是图中深蓝色部分。

## 输入格式

输入文件包含仅包含一组测试数据。

每组测试数据第一行为两个整数 $n,r$，其中 $n$ 表示了多边形的顶点个数，$r$ 表示了污染区域的半径。

接下来 $n$ 行，每行包含两个整数 $(x_i,y_i)$ ，表示每个顶点的坐标，以逆时针顺序给出；

数据保证多边形不自交或触及自身，没有顶点会位于圆弧上。

## 输出格式

输出多边形被圆心位于原点，半径为 $r$ 的半圆覆盖的面积。

答案的绝对误差不得超过 $10^{-3}$。

```input1
6 10
-8 2
8 2
8 14
0 14
0 6
-8 14
```

```output1
101.576437872
```

## 数据规模与约定

对于 $100\%$ 的数据，$3\leq n\leq 100$，$1\leq r\leq 10^3$，$-1.5\times 10^3 \leq x_i \leq 1.5\times 10^3$，$0\leq y_i\leq 1.5\times 10^3$。
