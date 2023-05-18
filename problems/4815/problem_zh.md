## 题目描述


小 Q 是个程序员。

作为一个年轻的程序员，小 Q 总是被老 C 欺负，老 C 经常把一些麻烦的任务交给小 Q 来处理。每当小 Q 不知道如何解决时，就只好向你求助。

为了完成任务，小 Q 需要列一个表格，表格有无穷多行，无穷多列，行和列都从 $1$ 开始标号。为了完成任务，表格里面每个格子都填了一个整数，为了方便描述，小 Q 把第 $a$ 行第 $b$ 列的整数记为 $f(a,b)$ 。为了完成任务，这个表格要满足一些条件：

1. 对任意的正整数 $a,b$，都要满足 $f(a,b) =f(b,a)$；
2. 对任意的正整数 $a,b$，都要满足 $b\times  f(a,a+b)=(a+b)\times   f(a,b)$ 。

为了完成任务，一开始表格里面的数很有规律，第 $a$ 行第 $b$ 列的数恰好等于 $a\times  b$，显然一开始是满足上述两个条件的。为了完成任务，小 Q 需要不断的修改表格里面的数，每当修改了一个格子的数之后，为了让表格继续满足上述两个条件，小 Q 还需要把这次修改能够波及到的全部格子里都改为恰当的数。由于某种神奇的力量驱使，已经确保了每一轮修改之后所有格子里的数仍然都是整数。为了完成任务，小 Q 还需要随时获取前k行前k列这个有限区域内所有数的和是多少，答案可能比较大，只需要算出答案 $\bmod 1000000007 $ 之后的结果。

## 输入格式

输入文件第1行包含两个整数 $m,n$ ，表示共有 $m$ 次操作，所有操作和查询涉及到的行编号和列编号都不超过 $n$。

接下来 $m$ 行，每行 $4$ 个整数 $a,b,x,k$，表示把第 $a$ 行 $b$ 列的数改成 $x$，然后把它能够波及到的所有格子全部修改，保证修改之后所有格子的数仍然都是整数，修改完成后计算前 $k$ 行前 $k$ 列里所有数的和。

## 输出格式

输出共 $m$ 行，每次操作之后输出一行，表示答案 $\bmod {1000000007}$ 之后的结果。

## 样例输入 #1

```plain
3 3
1 1 1 2
2 2 4 3
1 2 4 2
```

## 样例输出 #1

```plain
9
36
14
```

## 样例输入 #2

```plain
4 125
1 2 4 8
1 3 9 27
1 4 16 64
1 5 25 125
```

## 样例输出 #2

```plain
2073
316642
12157159
213336861
```

## 样例解释

【输入样例输出 1 说明】

一开始，表格的前 $3$ 行前

一开始，表格的前 $3$ 行前 $3$ 列如图中左边所示。前 $2$ 次操作后表格没有变化，第 $3$ 次操作之后的表格如右边所示。

```plain
1 2 3 2 4 6
2 4 6 4 4 12
3 6 9 6 12 9
```

对于 $100\%$ 的测试点，$1 \le  m \le  10^4$，$ 1 \le  a,b,k \le  n \le  4\times  10^6$，$ 0 \le  x < 10^{18}$。

![](https://cdn.luogu.com.cn/upload/pic/5012.png)
