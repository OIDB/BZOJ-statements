## 题目描述
FJ 决定为他的所有奶牛都配备手机，以此鼓励她们互相交流。不过，为此 FJ 必须在奶牛们居住的 $n$ 块草地中选一些建上无线电通讯塔，来保证任意两块草地间都存在手机信号。所有的 $n$ 块草地按 $1\sim n$ 顺次编号。 所有草地中只有 $n-1$ 对是相邻的，不过对任意两块草地 $a$ 和 $b$（$1 \leq a \leq n$，$1 \leq v \leq n$，$a \not= b$），都可以找到一个以 $a$ 开头以 $b$ 结尾的草地序列，并且序列中相邻的编号所代表的草地相邻。无线电通讯塔只能建在草地上，一座塔的服务范围为它所在的那块草地，以及与那块草地相邻的所有草地。 请你帮 FJ 计算一下，为了建立能覆盖到所有草地的通信系统，他最少要建多少座无线电通讯塔。

## 输入格式
* 第一行：一个整数 $n$

* 第 $2\sim n$ 行：每行为两个用空格隔开的整数 $a,b$，为两块相邻草地的编号

## 输出格式
* 第一行：输出一个整数，即 FJ 最少建立无线电通讯塔的数目

```input1
5
1 3
5 2
4 3
3 5
```
```output1
2
```
## 数据规模与约定
对于 $100\%$ 的数据，$1 \leq n \leq 1\times10^4$，$1 \leq a \leq n$，$1 \leq v \leq n$，$a \not= b$
## 提示
样例中 FJ 的农场中有 $5$ 块草地：草地 $1$ 和草地 $3$ 相邻，草地 $5$ 和草地 $2$、草地 $4$和草地 $3$，草地 $3$ 和草地 $5$ 也是如此。更形象一些，草地间的位置关系大体如下：

               4  2

               |  |

            1--3--5

FJ可以选择在草地2和草地3，或是草地3和草地5上建通讯塔。

## 题目来源
Usaco2008 Jan Gold