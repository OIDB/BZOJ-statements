## 题目描述

给定 $m$ 个素数和 $q$ 个询问。每个询问有 $n$ 个人，每次操作可以任意选择其中的一个素数 $p$（素数可以重复使用），然后去掉剩余人数 $\mod p$ 个人。对于每个询问，我们想知道，至少需要多少步操作才能去掉所有人。

## 输入格式

第一行：素数个数 $m$ 和询问个数 $q$。

第二行： $m$ 个素数 $p_i$。

下面 $Q$ 行：$n$。

## 输出格式

$Q$ 行答案。如果无解，输出 `oo`。



```input1
2 2
2 3
5
6
```



```output1
3
oo
```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le m,q \le 10^5$，$1 \le n \le 10^7$，$2 \le p_i \le 10^7$。

## 题目来源

abcdabcd987 提供
