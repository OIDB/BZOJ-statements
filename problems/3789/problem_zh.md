## 题目描述

$n$ 个城市和 $m$ 条单向道路构成一个有向图，每条道路 $e$ 上有整数积雪量 $w_e$。一辆扫雪车每天从城市 $s$ 开到 $t$，经过一条道路一次就将其雪量减 $1$（不能走雪量为 $0$ 的道路）。有些道路（称为重要道路）必须清空积雪，这些道路的导出子图是包含 $s$ 的弱连通图。求扫雪车工作天数的最大值，或判断无解。

弱连通图：将有向图的所有的有向边替换为无向边，所得到的图称为原图的基图。如果一个有向图的基图是连通图，则有向图是弱连通图。

## 输入格式

第一行四个数 $n,m,s,t$。

下面 $m$ 行，每行四个数 $x,y,w,t$。表示这条道路连接的两个城市，积雪量，和道路种类。若 $t$ 为 $0$ 则是普通道路，$t$ 为 $1$ 则是重要道路。

## 输出格式

扫雪车工作天数的最大值。或判断无解，输出 `0`。

```input1
4 7 1 4 
1 2 3 1 
2 1 100 0 
2 4 1 0 
1 3 1 0 
3 4 4 0 
2 3 2 1 
1 4 2 0
```

```output1
6
```

## 数据规模与约定

对于 $100\%$ 的数据，$2 \le n \le 100$，$0 \le m \le 5 \times 10^3$，$1 \le s,t \le n$，$s \ne t$，$1 \le x_i,y_i \le n$，$x_i \ne y_i$，$0 \le w_i \le 100$，$0 \le t_i \le 1$。
