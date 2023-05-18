## 题目描述

晓华所在的工作组正在编写一套高精度科学计算的软件，一些简单的部分如高精度加减法、乘除法早已写完了，现在就剩下晓华所负责的部分：实数的高精度开 $m$ 次根。因为一个有理数开根之后可能得到一个无理数，所以这项工作是有较大难度的。

现在要做的只是这项工作的第一步：只对自然数进行开整数次根，求出它的一个非负根，并且不考虑结果的小数部分，只要求把结果截断取整即可。程序需要根据给定的输入，包括需要开根的次数，以及被开根的整数；计算出它的非负根取整后的结果。

## 输入格式

共有两行，每行都有一个整数，并且输入中没有多余的空格：第一行有一个正整数 $m$，表示要开的根次

第二行有一个整数 $n$，表示被开根的数。

## 输出格式

只有一行，包括一个数，即为开根取整后的结果。

## 样例输入

```
3
1000000000
```

## 样例输出

```
1000
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le m\le 50$，$0\le n\le 10^{10000}$。
