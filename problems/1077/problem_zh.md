## 题目描述

你有 $n$ 个砝码，均为 $1$ 克，$2$ 克或者 $3$ 克。你并不清楚每个砝码的重量，但你知道其中一些砝码重量的大小关系。

你把其中两个砝码 $A$ 和 $B$ 放在天平的左边，需要另外选出两个砝码放在天平的右边。

问：有多少种选法使得天平的左边重（$c1$）、一样重（$c2$）、右边重（$c3$）？（只有结果保证惟一的选法才统计在内)

## 输入格式

第一行包含三个正整数 $n,A,B$（$1\le A,B\le n$，$A$ 和 $B$ 不相等）。砝码编号为 $1\sim N$。以下 $n$ 行包含重量关系矩阵，其中第 $i$ 行第 $j$ 个字符为加号 `+` 表示砝码 $i$ 比砝码 $j$ 重，减号 `-` 表示砝码 $i$ 比砝码 $j$ 轻，等号 `=` 表示砝码 $i$ 和砝码 $j$ 一样重，问号 `?` 表示二者的关系未知。存在一种情况符合该矩阵。

## 输出格式

仅一行，包含三个整数，即 $c1$，$c2$ 和 $c3$。

```input1
6 2 5
?+????
-?+???
?-????
????+?
???-?+
????-?
```

```output1
1 4 1
```

## 数据规模与约定
对于 $100\%$ 的数据，$4\le n\le 50$。


