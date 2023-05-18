## 题目描述

MST（最小生成树）：对于无向带权图 $<V,E>$，若其导出子图的边权和最小，且原图 $V$ 中对应的任意两个顶点间有且仅有一条通路，则称此图为原图的MST。  
你的任务很简单，对于给定的有向带权图，求出其“最小生成树”，即指定一个根以后，每个点都是从根出发可达的。
 
## 输入格式

输入文件最多包含 $3$ 组测试数据，对于每组测试数据：  
第一行为两个数 $n,m$，表示有向带权图的顶点数和边数，点编号为 $1～n$。  
接下来 $n$ 行，每行两个整数 $X_i,Y_i$，表示 $i$ 个顶点在直角坐标系中的坐标。  
接下来 $m$ 行，每行两个正整数 $x,y$，表示存在一条由点 $x$ 指向点 $y$ 的有向边，边权为两顶点的曼哈顿距离（定义见提示）。
 
## 输出格式

对于每组测试数据，输出一行：  
如果不存在“最小生成树”，输出 `Poor`；
否则输出最小边权和。

```input1
3 3
0 0
1 0
2 0
1 2
1 3
2 3
3 2
0 0
1 0
2 0
1 2
3 2
```

```output1
2
Poor
```

## 数据规模与约定

$100\%$ 的数据满足：$n \le 1 \times 10^3,m≤n^2,0 \le X_i,Y_i \le 1 \times 10^4$。

## 提示

对于两个点 $(a,b),(c,d)$，它们的曼哈顿距离定义如下：  
$l=|a-c|+|b-d|$  
可能存在自环。

## 题目来源

鸣谢 Hewr

