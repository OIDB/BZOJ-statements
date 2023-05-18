## 题目描述

给定三个小写字母串 $S_1,S_2,S_3$，其中有一些位置模糊不清了，用 `?` 代替。

你需要计算有多少种在每个 `?` 处都填入一个小写字母的方法，可以使得它们的字典序满足 $S_1<S_2<S_3$。

方案数对 $10^9+9$ 取模。

## 输入格式

多测。

第一行一个整数 $T$ 表示数据组数。

接下来 $T$ 组，每组三行三个字符串分别代表 $S_1,S_2,S_3$。

## 输出格式

对于每组数据输出一行一个整数表示答案对 $10^9+9$ 取模后的值。

```input1
3
?heoret?cal
c?mputer
?cience
jagiellonia
?niversity
kra?ow
?
b
c
```

```output1
42562
52
1
```

## 数据规模与约定

对于 $100\%$ 的数据，$\sum |S|\leq 10^6$。
