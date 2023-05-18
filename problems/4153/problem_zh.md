## 题目描述

有 $n$ 对夫妇,一开始夫妇之间互不认识,若两男或两女成为朋友，称他们为“熟人”，“熟人”关系具有传递性，即若 $a$ 熟 $b$ 且 $b$ 熟 $c$ 则 $a$ 熟 $c$。若两组夫妇的丈夫互相为熟人且妻子也相互为熟人则称他们为“熟悉的一对”。

现在给出 $q$ 个事件，每个事件会使得两男或两女成为朋友，并在每次事件之后计算“熟悉的一对”的个数。

## 输入格式

第一行一个数 $T$，表示数据组数。

接下来一行两个整数 $n,q$ 表示对数和事件数。

接下来 $q$ 行，每行三个整数 $t,a,b$，若 $t=1$，表示男 $a$ 和男 $b$ 成为朋友，$t=2$，表示女 $a$ 和女 $b$ 成为朋友。

## 输出格式

设当前是第 $i$ 个操作，$y_i$ 为本次事件之后的答案，令 $z_i=i\times y_i$，请输出 $z_1+z_2+...+z_q$ 模 $10^9+7$ 之后的值。

```input1
1
3 5
1 1 2
2 1 3
1 2 3
1 3 1
2 2 1
```

```output1
22
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq T\leq 8$，$1\leq n,q\leq 10^6$。
