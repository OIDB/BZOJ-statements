## 题目描述

Alice 和 Bob 居住在一个由 $n$ 座岛屿组成的国家，岛屿被编号为 $0$ 到 $n-1$。某些岛屿之间有桥相连，桥上的道路是双向的，但一次只能供一人通行。其中一些桥由于年久失修成为危桥，最多只能通行两次。

Alice 希望在岛屿 $a_1$ 和 $a_2$ 之间往返 $a_n$ 次（从 $a_1$ 到 $a_2$ 再从 $a_2$ 到 $a_1$ 算一次往返）。同时，Bob 希望在岛屿 $b_1$ 和 $b_2$ 之间往返 $b_n$ 次。这个过程中，所有危桥最多通行两次，其余的桥可以无限次通行。请问 Alice 和 Bob 能完成他们的愿望吗？

## 输入格式

本题有多组测试数据。

每组数据第一行包含 $7$ 个空格隔开的整数，分别为 $n,a_1,a_2,a_n,b_1,b_2,b_n$。

接下来是一个 $n$ 行 $n$ 列的对称矩阵，由大写字母组成。矩阵的 $i$ 行 $j$ 列描述编号 $i - 1$ 和 $j-1$ 的岛屿间的连
接情况，若为 `O` 则表示有危桥相连：为 `N` 表示有普通的桥相连：为 `X` 表示没有桥相连。

## 输出格式

对于每组测试数据输出一行，如果他们都能完成愿望输出 `Yes`，否则输出 `No`。

```input1
4 0 1 1 2 3 1
XOXX
OXOX
XOXO
XXOX
4 0 2 1 1 3 2
XNXO
NXOX
XOXO
OXOX
```
```output1
Yes
No
```

## 数据范围

$4 \le N < 50$  
$0 \le a_1, a_2, b_1, b_2 \le n-1$  
$1 \le a_n,b \le 50$
