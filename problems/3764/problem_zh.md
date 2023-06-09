## 题目描述

幸运数字是那些仅由 $4$ 和 $7$ 构成的数字，比如 $477,44,777$ 是幸运数字，而 $789,457,123$ 不是幸运数字。

有一天 Petya 得到了一个长度为 $n$ 的非负整数序列 $a$ ，其中 $a_i$ 表示该序列的第 $i$ 个元素。他想从整个序列中选出两个互不相交的子段 $a_{l_1 \sim r_1},a_{l_2 \sim r_2}$，使得不存在某个幸运数字既在 $a_{l_1 \sim r_1}$ 出现，又在 $a_{l_2\sim r_2}$ 出现。 Petya 想知道他有多少种选择方案，你能帮帮他吗？

Petya 保证 $a$ 序列中幸运数字的总出现次数不会超过 $10^3$ 次。

## 输入格式

输入的第一行包含一个正整数 $n$，表示 $a$ 序列的长度。  
第二行包含 $n$ 个整数，第 $i$ 个整数表示 $a_i$。

## 输出格式

输出一行表示总的方案个数。

```input1
4
1 4 2 4
```

```output1
9
```

## 数据规模与约定

对于 $100\%$ 的数据，$n \le 10^5$，$1 \le l_1 \le r_1 \le n$，$1 \le l_2 \le r_2 \le n$，幸运数字的总出现次数不超过 $10^3$。

此题存在版权，故原 BZOJ 不再支持提交，保留在此只供大家参考题面！ 望见谅！

