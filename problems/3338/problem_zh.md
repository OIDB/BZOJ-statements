


## 题目描述
Solitaire is a game played on a chessboard 8x8. The rows and columns of the chessboard are numbered from 1 to 8, from the top to the bottom and from left to right respectively.
There are four identical pieces on the board. In one move it is allowed to:
> move a piece to an empty neighboring field (up, down, left or right),
> jump over one neighboring piece to an empty field (up, down, left or right). 
There are 4 moves allowed for each piece in the configuration shown above. As an example let's consider a piece placed in the row 4, column 4. It can be moved one row up, two rows down, one column left or two columns right.
Write a program that:
> reads two chessboard configurations from the standard input,
> verifies whether the second one is reachable from the first one in at most 8 moves,
> writes the result to the standard output.
**在一个8*8的棋盘上,方上4颗相同的棋子,每次可以将其中一颗棋子上下左右移动一格;如果有阻碍,也可以跳过一颗棋子.按照这样的移动规则,问是否能从给定的一种棋盘状态在8步之内移动到另一种状态** 
## 输入格式
**Each of two input lines contains 8 integers a1, a2, ..., a8 separated by single spaces and describes one configuration of pieces on the chessboard. Integers a2j-1 and a2j (1 <= j <= 4) describe the position of one piece - the row number and the column number respectively. Process to the end of file.** 
## 输出格式
**The output should contain one word for each test case - YES if a configuration described in the second input line is reachable from the configuration described in the first input line in at most 8 moves, or one word NO otherwise.** 

```input14 4 4 5 5 4 6 5
2 4 3 3 3 6 4 6

```

```output1YES
```

## 提示
没有写明提示
## 题目来源
双向BFS


