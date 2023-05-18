## 题目描述

五子棋是一种流传很广的棋类游戏，在一个 $15\times 15$ 的棋盘上，对弈双方执黑白棋子（类似于围棋），执黑子者先下，凡落下的棋子不能被提起，即不存在挪子和吃子的情况。为了简化问题，假设黑方不存在「禁手」，「禁手」是五子棋术语，指禁止走棋子的地方。当某选手的棋子在横、竖、$45$ 度斜线方向、$135$ 度斜线方向之一先出现相连的 $5$ 个棋子时，该选手获胜。先考虑轮到黑棋走的一盘残局，请给出黑棋获胜的最少步数和在该步数下能获胜的所有不同的下一步走法。

## 输入格式

输入文件中共有 $15$ 行，每行有 $15$ 个由一个空格隔开的整数。

第 $i$ 行，第 $j$ 列的整数记做 $v_{i,j}$，用 $v_{i,j}=0，1，2$ 表示第 $i$ 行，第 $j$ 列的位置为空、有一黑子、有一白子，从左上角开始，按从左至右，自上而下的顺序输入，即输入的第一行第一列整数 $v_{1,1}$ 表示第一行第一列位置的状态，输入的第 $15$ 行第 $15$ 列整数 $v_{15,15}$ 表示第 $15$ 行第 $15$ 列位置的状态。

## 输出格式

输出文件中的第一行为两个整数 $a$ 和 $b$，其中：$a$ 表示黑棋获胜的最少步数，$b$ 表示黑棋在 $a$ 步获胜的所有不同的下一步走法的种数。

从第二行到第 $b+1$ 行，每行有两个整数，分别表示黑棋在 $a$ 步获胜的一种下一步走法落子位置的行数 $i$ 和列数 $j$，要求这些走法按照 $15i+j$ 的大小从小到大排列。

```input1
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 0 0 2 0 0 0 0 0
0 0 0 0 0 0 0 2 0 2 0 0 0 0 0
0 0 0 0 0 0 2 1 1 2 0 0 0 0 0
0 0 0 0 0 0 0 1 2 1 0 0 0 0 0
0 0 0 0 0 0 2 1 1 1 1 2 0 0 0
0 0 0 0 0 0 0 1 0 1 0 1 0 0 0
0 0 0 0 0 0 2 2 0 1 1 0 2 0 0
0 0 0 0 0 0 0 0 0 2 0 2 0 0 0
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
```

```output1
3 2
10 9
10 11
```

## 题目来源

数据由 SillyHook 生成