## 题目描述

![](https://hydro.ac/d/bzoj/p/1608/file/pic1.jpg)

## 输入格式

第 $1$ 行是两个整数 $r$ 和 $c$，用空格隔开。从第 $2$ 行到第 $r\times c +1$  行，每一行包含 $1$ 个数字和 $4$ 个代表边界的符号（可以是字母或数字 $0$）。

## 输出格式

输出换位及旋转后的拼图。共 $R \times C$ 行，每行第一个数字代表第几块拼图块，后面四个字符，按顺序代表 $4$ 个边界字母（边界线仍用 $0$ 表示）。答案可能有多组，输出一组即可。

## 样例输入

```input1
2 3
1 c d 0 0
2 0 d b 0
3 c 0 d a
4 b a b 0
5 d 0 0 e
6 0 0 b e
```



```output1
1 0 c d 0
3 0 d a c
5 0 0 e d
2 d b 0 0
4 a b 0 b
6 e 0 0 b
```



## 数据规模与约定

$1 \leq R,C \leq 10 $

## 题目来源

$\text{Silver}$