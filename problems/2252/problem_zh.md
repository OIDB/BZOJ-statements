## 题目描述

假设我们有矩阵，其元素值非 $0$ 即 $1$。

**$a_{1,1} \dots\dots a_{1,m}$**

**$\dots\dots\dots\dots\dots$**

**$a_{n,1} \dots\dots a_{n,m}$**

定义 $a_{i,j}$ 与 $a_{k,l}$ 之间的距离为 $D(a_{i,j},a_{k,l})=abs(i-k)+abs(j-l)$。

## 输入格式

输入文件的第一行为两个整数，分别代表 $n$ 和 $m$。

接下来的 $n$ 行，第 $i$ 行的第 $j$ 个字符代表 $a_{i,j}$。

## 输出格式

输出包含 $n$ 行，每行 $m$ 个用空格分开的数字，其中第 $i$ 行第 $j$ 个数字代表：

$Min(D(a_{i,j},a_{x,y}))$（$1 \le x \le n$，$1 \le y ＜ m$，且 $a_{x,y}=1$）

```input1
3 4
0001
0011
0110
```

```output1
3 2 1 0
2 1 0 0
1 0 0 1
```

## 数据规模与约定

$100\%$ 的数据满足：$0 \le m,n \le 1 \times 10^3$。