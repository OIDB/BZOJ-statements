## 题目描述

小园丁 Mr. S 负责看管一片田野，田野可以看作一个二维平面。田野上有 $n$ 棵许愿树，编号 $1,2,3,\dots,n$，每棵树可以看作平面上的一个点，其中第 $i$ 棵树 $(1\le i\le n)$ 位于坐标 $(x_i,y_i)$。任意两棵树的坐标均不相同。

老司机 Mr. P 从原点 $(0,0)$ 驾车出发，进行若干轮行动。每一轮，Mr. P 首先选择任意一个满足以下条件的方向：为左、右、上、左上 $45^\circ$、右上 $45^\circ$ 五个方向之一。沿此方向前进可以到达一棵他尚未许愿过的树。

完成选择后，Mr. P 沿该方向直线前进，必须到达该方向上距离最近的尚未许愿的树，在树下许愿并继续下一轮行动。如果没有满足条件的方向可供选择，则停止行动。他会采取最优策略，在尽可能多的树下许愿。若最优策略不唯一，可以选择任意一种。

不幸的是，小园丁 Mr. S 发现由于田野土质松软，老司机 Mr. P 的小汽车在每轮行进过程中，都会在田野上留下一条车辙印，一条车辙印可看作以两棵树（或原点和一棵树）为端点的一条线段。

在 Mr. P 之后，还有很多许愿者计划驾车来田野许愿，这些许愿者都会像 Mr. P 一样任选一种最优策略行动。Mr. S 认为非左右方向（即上、左上 $45^\circ$、右上 $45^\circ$ 三个方向）的车辙印很不美观，为了维护田野的形象，他打算租用一些轧路机，在这群许愿者到来之前夯实所有「可能留下非左右方向车辙印」的地面。

「可能留下非左右方向车辙印」的地面应当是田野上的若干条线段，其中每条线段都包含在某一种最优策略的行进路线中。每台轧路机都采取满足以下三个条件的工作模式：

1. 从原点或任意一棵树出发。

2. 只能向上、左上 $45^\circ$、右上 $45^\circ$ 三个方向之一移动，并且只能在树下改变方向或停止。

3. 只能经过“可能留下非左右方向车辙印”的地面，但是同一块地面可以被多台轧路机经过。

现在 Mr. P 和 Mr. S 分别向你提出了一个问题:

请给 Mr .P 指出任意一条最优路线。

请告诉 Mr. S 最少需要租用多少台轧路机。

## 输入格式

输入文件的第一行包含一个正整数 $n$，表示许愿树的数量。

接下来 $n$ 行，第 $i+1$ 行包含两个整数 $x_i,y_i$，中间用单个空格隔开，表示第 $i$ 棵许愿树的坐标。

## 输出格式

输出文件包括三行。

输出文件的第一行输出一个整数 $m$，表示 Mr. P 最多能在多少棵树下许愿。

输出文件的第二行输出 $m$ 个整数，相邻整数之间用单个空格隔开，表示 Mr. P 应该依次在哪些树下许愿。

输出文件的第三行输出一个整数，表示 Mr. S 最少需要租用多少台轧路机。

## 样例

```input1
6
-1 1
1 1
-2 2
0 8
0 9
0 10
```
```output1
3
2 1 3
3
```

## 样例说明

最优路线共 $2$ 条可许愿 $3$ 次：$(0,0)\rightarrow(1,1)\rightarrow(−1,1)\rightarrow(−2,2)$ 或 $(0,0)\rightarrow(0,8)\rightarrow(0,9)\rightarrow(0,10)$。

至少 $3$ 台轧路机，路线是 $(0,0)\rightarrow(1,1)$，$(−1,1)\rightarrow(−2,2)$ 和 $(0,0)\rightarrow(0,8)\rightarrow(0,9)\rightarrow(0,10)$。

## 数据规模与约定

![](https://hydro.org.cn/d/bzoj/p/4200/file/4200.png)

对于所有数据，$n\le 5\times 10^4$，$|x_i|\le 10^9$，$0<y_i\le 10^9$。

对于每个测试点：

若输出文件的第一行正确，得到该测试点 $20\%$ 的分数；

若输出文件的前两行正确，得到该测试点 $40\%$ 的分数；

若输出文件完全正确，得到该测试点 $100\%$ 的分数。