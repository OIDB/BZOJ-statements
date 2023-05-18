## 题面描述
数轴上有 $n$ 个石子，第 $i$ 个石头的坐标为 $D_i$ , 现在从位置 $0$ 开始，跳到位置 $L$ ，每次跳都从一个石子跳到相邻的下一个石子，现在 $FJ$ 允许你移走 $M$ 个石子，问移走这 $M$ 个石子后相邻两个石子距离的最小值的最大值是多少？ 

## 输入格式
第一行：三个整数 $ L , N , M $ ， $L$ 代表一个位置，是要跳到的最终坐标， $N$ 代表有 $N$ 个石子 ， $M$ 代表可以移走 $M$ 个石子。

接下来 $N$ 行，第 $i$ 行一个整数 $D_i$ 表示第 $i$ 个石头距离起点的距离。
## 输出格式
输出一行一个整数，表示在移走 $M$ 个石子后香玲两个石子距离的最小值的最大值。
## 样例输入
```
25 5 2
2
14
11
21
17
```
## 样例输出
```
4
```
## 样例说明
移除之前，最短距离在位置 $2$ 的石头和起点之间；移除位置 $2$ 和位置 $14$ 两个石头后，最短距离变成 $17$ 和 $21$ 或 $21$ 和 $25$ 之间的 $4$ 。
## 数据规模与约定
对于 100\% 的数据 $1 \leq L \leq 10^9$ , $1 \leq M\leq N \leq 5\times10^4$ 。