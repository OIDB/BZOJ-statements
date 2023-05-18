## 题目背景

《星际争霸 2》全面公测啦！

## 题目描述

《星际争霸 2》的游戏目标就是在战役中打败你对手的军队。

一支军队由 $3$ 种单位组成，不同单位有不同的**实数**力量值：cattlebruisers 的力量是 $S_1$，cow templars 的力量是 $S_2$，ultracows 的力量是 $S_3$。一支军队的力量值，是其中各的单位的力量值之和：比如一支军队有 $23$ 个 cattlebruisers，那么这支军队单独从 cattlebruisers 就能获得 $23S_1$ 的力量值。

当两支对立的军队在战役中厮杀，**力量值更高**的军队会获得胜利。如果两支军队的力量值恰好相同，那么将**随机**产生一个获胜方。

Farmer John 和 Bessie 进行了 $N$ 局测试战役。在第 $i$ 局测试战役中，Farmer John 有 $J_{1,i}$ 个 cattlebruisers，$J_{2,i}$ 个 cow templars，以及 $J_{3,i}$ 个 ultracows。Bessie的军队有 $B_{1,i}$ 个 cattlebruisers，$B_{2,i}$ 个 cow templars 以及 $B_{3,i}$ 个 ultracows。每局战役后，将胜者以一个单独的“胜利字母” $V_i$ 记录下来：`J` 表示 Farmer John 获胜，而 `B` 表示 Bessie 获胜。这是他们唯一所拥有的信息。

他们不知道自己军队具体的力量值是多少，现在他们希望仅根据这 $N$ 局测试战役来预测一些另外的战役的结果。给出这 $N$ 场测试战役的结果，写一个程序来确定另外 $M$ 场战役的获胜方。

保证所有给出的测试战役的结果都是正确的，即至少存在一种合法的力量值的取值符合这些结果，没有一个单位的力量值超过另一个单位力量值的 $100$ 倍。

## 输入格式

第一行：两个用空格隔开的整数 $N$ 和 $M$。

第 $2$ 到第 $N+1$ 行：第 $i+1$ 行：第一个是胜利字母 $V_i$，接下来是 $6$ 个整数：$J_{1_i},J_{2,i},J_{3,i},B_{1,i}, B_{2,i},B_{3,i}$。

第 $N+2$ 到第 $N+M+1$ 行: 第 $i+N+1$ 行给出 $6$ 个整数 $J_{1_i},J_{2,i},J_{3,i},B_{1,i}, B_{2,i},B_{3,i}$ 表示第 $i$ 场额外战役。

## 输出格式

共 $M$ 行，第 $i$ 行包含第 $i$ 场额外战役的结果：`J` 表示 Farmer John 一定能赢，`B` 表示 Bessie 一定能赢，`U` 表示不确定，也就是不可能利用给出的信息推断出谁一定能获胜。

```input1
3 3
J 6 5 4 5 4 7
B 5 4 2 3 5 5
J 9 0 10 8 2 7
6 6 4 5 4 7
9 0 10 8 2 6
3 4 8 4 4 6

```

```output1
J
J
U
```

## 提示

一开始的两场战役已经在题目中给出过解释了。最后一场战役是不能利用已有信息推断出结果的。

具体来说，对于 S_1=9.0, S_2=7.0, S_3=4.0 和 S_1=12.0, S_2=20.0, S_3=10.0 

这两组不同的数值都符合输入信息，但是却能使的最后一场测试战役产生不同的结果。

## 题目来源
Gold