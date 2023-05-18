## 题目描述

Alice 和 Bob 两个好朋友又开始玩取石子了。游戏开始时，有 $n$ 堆石子排成一排，然后他们轮流操作（Alice先手），每次操作时从下面的规则中任选一个：

- 从某堆石子中取走一个。
- 合并任意两堆石子。

先不能操作的人输。Alice 想知道，她是否能有必胜策略。

## 输入格式

**本题存在多组数据。**

第一行输入 $T$，表示数据组数。

对于每组测试数据，第一行读入 $n$。

接下来 $n$ 个正整数 $a_1,a_2\dots a_n$，表示每堆石子的数量。

## 输出格式

对于每组测试数据，输出一行。

输出 `YES` 表示 Alice 有必胜策略，输出 `NO` 表示 Alice 没有必胜策略。

```input1
3
3
1 1 2
2
3 4
3
2 3 5
```

```output1
YES
NO
NO
```

## 数据规模与约定

对于 $100\%$ 的数据，$T\le100$，$n\le50$，$a_i\le10^3$。