## 题目描述

某天，wangxz 神犇来到了一个信息学在线评测系统（Online Judge）。由于他是一位哲♂学的神犇，所以他不打算做题。他发现这些题目呈线性排列，被标记为 $1-n$ 号，每道题都有一个难度值（可以 $\le 0$）。他决定与这些题目玩♂耍。

1. 他可以在某个位置插♂入一些难度值特定的题目。
2. 他可以吃♂掉（删除）一段题目。
3. 他可以查询某个位置的题目的难度值。

维护一个初始有 $n$ 个元素的序列(标记为 $1-n$ 号元素)，支持以下操作：

- `0 p a b`（$0\le p\le 当前序列元素个数,a\le b$）在 $p$ 位置和 $p+1$ 位置之间插入整数：$a,a+1,a+2,...,b-1,b$。若 $p$ 为 $0$，插在序列最前面;
- `1 a b`（$1\le a\le b\le 当前序列元素个数$）删除 $a,a+1,a+2,...,b-1,b$ 位置的元素;
- `2 p`（$1\le p\le 当前序列元素个数$）查询 $p$ 位置的元素。

## 输入格式

输入第一行包括两个正整数$n,m$，代表初始序列元素个数和操作个数。
接下来 $n$ 个整数,为初始序列元素。
接下来 $m$ 行,每行第一个为整数 $sym$,
若 $sym=0$，接下来有一个非负整数 $p$，两个整数 $a,b$；
若 $sym=1$，接下来有两个正整数 $a,b$；
若 $sym=2$，接下来有一个正整数 $p$。

## 输出格式

对每个 $sym=2$，输出一行，包括一个整数，代表询问位置的元素。

```input1
5 3
1 2 3 4 5
0 2 1 4
1 3 8
2 2
```

```output1
2
```

## 数据规模与约定

$1\le n,m\le 20000$，在任何情况下，保证序列中的元素总数不超过 $100000$。保证题目涉及的所有数在 $int$ 内。

## 题目来源

From LiZitong

