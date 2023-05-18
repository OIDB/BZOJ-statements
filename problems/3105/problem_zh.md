## 题目描述

传统的 Nim 游戏是这样的：有一些火柴堆，每堆都有若干根火柴（不同堆的火柴数量可以不同）。两个游戏者轮流操作，每次可以选一个火柴堆拿走若干根火柴。可以只拿一根，也可以拿走整堆火柴，但不能同时从超过一堆火柴中拿。拿走最后一根火柴的游戏者胜利。

本题的游戏稍微有些不同：在第一个回合中，第一个游戏者可以直接拿走若干个整堆的火柴。可以一堆都不拿，但不可以全部拿走。第二回合也一样，第二个游戏者也有这样一次机会。从第三个回合（又轮到第一个游戏者）开始，规则和 Nim 游戏一样。如果你先拿，怎样才能保证获胜？如果可以获胜的话，还要让第一回合拿的火柴总数尽量小。

## 输入格式

第一行为整数 $k$，即火柴堆数。第二行包含 $k$ 个整数 $a_i$，即各堆的火柴个数。

## 输出格式

输出第一回合拿的火柴数目的最小值。如果不能保证取胜，输出 `-1`。


```input1
6
5 5 6 6 5 5
```


```output1
21
```

## 数据规模与约定

对于 $100\%$ 的数据，保证 $1 \leq k \leq 100$，$1 \leq a_i \leq 10^9$。