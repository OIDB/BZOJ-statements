

## 题目描述
给定一个 $n\times n$ 的矩阵，每个单元矩阵有一种颜色。你需要按照这样一种规则移动魔方：

可以将任何一行（或一列）向左右（或上下）移动，并且如果向左边移动，那么移出魔方的单元矩阵将在右方按顺序出现。

游戏开始时，玩家会得到魔方的初始状态与目标状态，玩家需要把魔方按照规则移动到目标状态。

你需要报告问题是否有解。
## 输入格式
本题有多组数据。

第一行一个整数 $T$，表示输入数据组数。

接下来共有 $T$ 组数据。

每组数据第一行有一个整数 $n$，表示魔方的数量级。

接下来会给出两个魔方，分别表示魔方的初始状态与目标状态，其中颜色用不同的整数表示。
## 输出格式
对于每一组数据，如果有解则输出一行 `Yes`，否则输出一行 `No`。

```input1
2
3
1 2 3
4 5 6
7 8 9
2 1 3
4 5 6
7 8 9
6
1 1 2 3 3 4
4 1 1 4 2 3
3 3 1 1 1 4
3 4 4 3 4 3
4 3 4 4 3 3
3 3 3 3 4 2
1 1 2 3 3 3
2 3 4 1 1 2
3 3 1 1 1 4
3 4 4 3 4 4
4 3 4 4 3 4
3 3 3 3 4 3
```
```output1
No
Yes
```

## 提示
[数据范围]
对于 $100\%$ 的数据，$1\le T\le 15$，$1\le n\le 50$。
## 题目来源
没有写明来源

