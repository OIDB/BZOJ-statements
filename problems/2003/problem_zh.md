## 题目描述

小 Z 近日闲来无事，便研究起矩阵来。他先写了一个 $n\times m$ 的矩阵，每个格子里填入了一个小于 $p$ 的非负整数，然后他对于每个 $2\times 2$ 的子矩阵，算出了其中数的和。

譬如 $n=3, m=3, p=3$，小 Z 写的矩阵如下：
$$
a=
\begin{pmatrix}
0&1&2\\
1&2&0\\
2&0&1
\end{pmatrix}
$$

共有 $4$ 个 $2\times 2$ 的子矩阵，容易算出它们的和如下：

$$
s=
\begin{pmatrix}
0&0&0\\
0&4&5\\
0&5&3
\end{pmatrix}
$$

（第一行和第一列的 $0$ 是为了格式美观而添加进去的。）

现在小 Z 想试一试能不能根据这些和推算出原矩阵。由于小 Z 的数学并不好，因此这个任务就交给你了。

当然，小 Z 早就发现了，解很可能不唯一，譬如下面的矩阵算出的和与 $a$ 相同：

$$
b=
\begin{pmatrix}
0&2&1\\
0&2&0\\
2&1&0
\end{pmatrix}
$$

示意图在有多个矩阵满足要求的情况下请你输出字典序最小的那一个。

字典序的比较方式如下：对于两个解矩阵 $x$ 和 $y$，找到 $x$ 和 $y$ 不同的位置中行数最小的那一个格子，若有多个则取列数最小的那个格子，该位置较小的矩阵字典序较小。

譬如上述的矩阵 $a$ 和 $b$，第一个不同的格子应是第一行第二个格子，而 $a_{1,2} < b_{1,2}$，故矩阵 $a$ 的字典序比 $b$ 小。另外，小 Z 的数学还没有差到加法都做错，因此保证输入数据都是有解的。

## 输入格式

第一行包含三个正整数 $n,m,p$ 表示矩阵的行数列数以及每个数的范围，接下来 $n$ 行每行包含 $m$ 个非负整数，其中第 $i$ 行第 $j$ 个数表示以格子 $(i,j)$ 为右下角的 $2 \times 2$ 子矩阵中的数的和。

## 输出格式

包含 $n$ 行，每行 $m$ 个整数，描述你求出的矩阵，相邻的整数用空格分开。（行末不要有多余空格。）

```input1
3 3 3
0 0 0
0 4 5
0 5 3
```
```output1
0 0 2
2 2 1
1 0 0
```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \leq n,m \leq 200$，$1 < p \leq 10$。数据的第一行与第一列的数均为 $0$，且每个和都不超过 $4(p-1)$。