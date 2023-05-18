## 题目描述

我们考虑的序列满足下列条件：

- 序列长度为 $c$，
- 序列中的每个元素都为 $1-9$，
- 序列中每个元素不重复出现。

一个单独的序列将被称为一个 code。

当对给定的两个 codes 估计他们的兼容性时，我们主要看两个值。第一个就是（column $a$）所有同时出现在两个 codes 中且出现在同一位置的数字的和，第二个就是（column $b$）所有同时出现在两个 codes 但出现在不同位置的数字和。

当我们给定 $c$ 个 codes 和他们于某个未知 code 的兼容性信息时。我们可以找到并把未知 code 表示出来。下面是一个 $c=3$ 的例子。

![](https://hydro.org.cn/d/bzoj/p/2604/file/pic1.jpg)

## 输入格式

第一行只有一个整数 $c$。接下来 $c$ 行每行给出了一个 code 和未知 code 的兼容信息，每行一个。

每行都有 $c+2$ 非负整数，第一个和第二个表示兼容信息，后面 $c$ 个数表示这个 code。

## 输出格式

输出合法的未知 code，数据保证一定有解，如果有多解，输出任意一个。

## 样例输入

```plain
3
4 0 4 9 7
0 10 6 7 4
0 5 9 4 1
```

## 样例输出

```plain
4 1 6
```

## 提示

请不要提交，希望有人提供 SPJ。

## 数据规模与规定

对于 $100\%$ 的数据，$1 \le c \le 9$。
