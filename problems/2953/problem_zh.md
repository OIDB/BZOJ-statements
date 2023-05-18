## 题目描述
某首都城市的商人要经常到各城镇去做生意，他们按自己的路线去做，目的是为了更好的节约时间。

假设有 $n$ 个城镇，首都编号为 $1$，商人从首都出发，其他各城镇之间都有道路连接，任意两个城镇之间如果有直连道路，在它们之间行驶需要花费 $1$ 单位时间。该国公路网络发达，从首都出发能到达任意一个城镇，并且公路网络不会存在环。

你的任务是帮助该商人计算一下他的最短旅行时间。
## 输入格式
第一行有一个整数 $n$，为城镇的数目。

接下来 $n-1$ 行，每行由两个整数 $a$ 和 $b$ 组成，表示城镇 $a$ 和城镇 $b$ 有公路连接。

接下来一行输入一个整数 $m$，代表城镇的数量。

接下来 $m$ 行，每行有该商人需要顺次经过的各城镇编号。
## 输出格式
输出一个整数，即该商人旅行的最短时间。
## 样例输入
```plain
5
1 2
1 5
3 5
4 5
4
1
3
2
5
```
## 样例输出
```plain
7
```
## 数据规模与约定
对于所有数据，$1\leq n\leq 3\times10^4$，$1\leq m\leq 5\times 10^3$。