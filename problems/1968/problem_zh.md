## 题目描述

科学家们在 Samuel 星球上的探险得到了丰富的能源储备，这使得空间站中大型计算机 Samuel II 的长时间运算成为了可能。由于在去年一年的辛苦工作取得了不错的成绩，小联被允许用 Samuel II 进行数学研究。

小联最近在研究和约数有关的问题，他统计每个正数 $n$ 的约数的个数，并以 $f(n)$ 来表示。例如 $12$ 的约数有 $1,2,3,4,6,12$，因此 $f(12)=6$。下表给出了一些 $f(n)$ 的取值：

| $n$    | $1$ | $2$ | $3$ | $4$ | $5$ | $6$ |
| -------- | ----- | ----- | ----- | ----- | ----- | ----- |
| $f(n)$ | $1$ | $2$ | $2$ | $3$ | $2$ | $4$ |

现在小联希望用 Samuel II 来统计 $f(1)$ 到 $f(m)$ 的累加和 $s$：

$$
s=\sum_{i=1}^m f(i)
$$

## 输入格式

只有一行一个整数 $m$。

## 输出格式

只有一行输出，为整数 $s$，即 $f(1)$ 到 $f(m)$ 的累加和。

```input1
3
```

```output1
5
```

## 数据规模与约定

对于 $100\%$ 的数据，$0 < m < 10^6$。
