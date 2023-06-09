## 题目描述

一个 $n \times n(n\ge2)$ 棋盘上有黑白棋子各一枚。游戏者A和B轮流移动棋子， A 先走。

1. A 的移动规则：只能移动白棋子。可以往上下左右四个方向之一移动一格。
2. B 的移动规则：只能移动黑棋子。可以往上下左右四个方向之一移动一格或者两格。

和通常的“吃子”规则一样，当某游戏者把自己的棋子移动到对方棋子所在的格子时，他就赢了。两个游戏者都很聪明，当可以获胜时会尽快获胜，只能输掉的时候会尽量拖延时间。你的任务是判断谁会赢，需要多少回合。比如 $n=2$，白棋子在 $(1,1)$，黑棋子在 $(2,2)$，那么虽然 A 有两种走法，第二个回合 B 总能取胜。

## 输入格式

仅一行，包含五个整数 $n, r1, c1, r2, c2$，即棋盘大小和棋子位置。 白色棋子在 $(r1,c1)$，黑色棋子在 $(r2,c2)$ $(1 \le r1,c1,r2,c2 \le n)$。黑白棋子的位置保证不相同。

## 输出格式

仅一行，即游戏结果。如果 A 获胜，输出 `WHITE x`；如果 B 获胜，输出 `BLACK x`；如果二者都没有必胜策略，输出 `DRAW`。


```input1
2 1 1 2 2
```


```output1
BLACK 2
```

## 数据规模与约定

对于 $100\%$ 的数据，$n\le 20$。
