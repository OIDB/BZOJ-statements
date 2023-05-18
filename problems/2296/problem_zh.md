## 题目描述

1tthinking 除了随机算法，其他什么都不会。但是他还是可以通过很多题目，他用的是什么呢？他会选择一个好的随机种子，然后输出答案。往往他选择的一个好的种子可以有 $99\%$ 的概率通过题目。

他会按照下面的规则选择一个种子。首先 1tthinking 有自己喜欢的一个幸运数字 $x$，然后他会找一个数字 $a$ 使得 $x|a$ 且 $a$ 的十进制表示包含 $[0,9]$ 的每一个数字。

举个例子，如果 $x=1$，那么 $9182736450$ 就是一个 1tthinking 需要的随机种子。

然而 1tthinking 有的时候花了很久也找不到这个数，他感到很失望。现在他把问题留给了你。

## 输入格式

第一行一个整数 $T$ 表示数据组数。

接下来 $T$ 行，每行一个整数 $x$ 表示一个幸运数字。

## 输出格式

共 $T$ 行，每行一个满足条件的随机种子，如果不存在，输出 `-1`。

数据保证如果存在答案，则答案不超过 $10^{16}$。

```input1
3
1
2
10
```

```output1
9876543210
9876543210
9876543210
```

## 数据规模与约定

对于 $100\%$ 的数据，$0\leq T\leq 100$，$0\leq x\leq 10^6$。
