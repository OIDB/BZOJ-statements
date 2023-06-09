## 题目描述

一个城市内有 $n$ 个地点需要夜间巡逻，而巡逻员只有 WZK 和他愉快的伙伴小 Y 两人。

为了分工明确，两个人各自被划分一块凸多边形的区域（区域可能退化成一条直线、一个点），这两块区域加起来必须覆盖这 $n$ 个地点。为了不在巡逻的时候吵起来，两个人负责的区域必须严格不相交。

WZK 很大方地让小 Y 决定两块区域的具体边界，但小 Y 知道，如果 WZK 负责的区域面积大于自己负责的面积，WZK 肯定会不同意，但是小 Y 又希望自己巡逻的区域尽量小一些，因此他向你寻求帮助。

## 输入格式

第一行，一个整数 $n (1\le n\le 50)$ 表示两块区域加起来必须覆盖的点的个数。

第二行，$n$ 个绝对值不超过 $10^3$ 的整数，表示这 $n$ 个点的横坐标。

第三行，$n$ 个绝对值不超过 $10^3$ 的整数，表示这 $n$ 个点的纵坐标。

## 输出格式

仅一行，为小 Y 负责的局域的面积的最小可行值，保留一位小数。

## 样例输入

```plain
5 
-1000 -1000 1000 1000 0 
-1000 1000 -1000 1000 0
```

## 样例输出

```plain
1000000.0
```

## 样例说明

一种最优的方案是 WZK 负责 $(-1000,-1000),(-1000,1000)$ 这两个点，这是一个面积为 $0$ 的退化成一条直线的区域，小 Y 负责 $(1000,-1000),(1000,1000),(0,0)$ 这三个点，这是一个面积为 $10^6$ 的三角形区域。

## 数据规模与约定

对于所有数据，$1\le n\le 50$ 且坐标的绝对值不超过 $10^3$。

