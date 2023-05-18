## 题目描述

小云和小南两姐妹从小喜欢下象棋，现在作为象棋高手的她们，已经不屑于玩平常的象棋了，于是她们便开始用棋盘和棋子玩各种各样的新游戏。

今天天气晴朗，阳光明媚，她们将在 $ n \times m $ 的棋盘上进行游戏。

棋盘上有 $ k $ 颗棋子和若干有障碍格子，令棋盘左上角格子坐标为 $ (1,1) $ ，右下角格子坐标为 $ (n, m) $ ，参数 $ a $ 、 $ b $ 规定了所有棋子的走法：在 $ (x, y) $ 的棋子下一步能走到 $ (x + a, y + b), (x + a, y - b), (x – a, y + b), (x – a, y – b), (x + b, y + a), (x + b, y - a), (x – b, y + a), (x – b, y – a) $ 这八个格子中的一个，棋子任何时候不能跃出棋盘或走到有障碍的格子上。

这 $ k $ 颗棋子是相同的，小云和小南的目标是用最少步数把所有棋子移动到特定格子，要求移动过程中不能出现多颗棋子同时在某一格的情况。

她们已经想出步数较少方案，但无法确定这是否为最少步数，所以向作为程序员的你求助。

## 输入格式

第一行五个空格隔开的整数 $ n $、$ m $、$ k $、$ a $ 以及 $ b $；

接下来 $ n $ 行，每行为长度m的字符串，描述棋盘，``.``表示没有障碍的格子，``*``表示有障碍的格子；

接下来 $ k $ 行，每行两个整数 $ x $ 和 $ y $ ，分别表示 $ k $ 颗棋子的初始位置；

接下来 $ k $ 行，每行两个整数 $ x $ 和 $ y $ ，分别表示 $ k $ 颗棋子的目标位置。

## 输出格式

一个整数，为把所有棋子移动到 ``t`` 位置的最少步数，数据保证有解。

## 样例输入

```
1 8 2 2 0
.......*
1 1
1 3
1 5
1 7
```

## 样例输出

```
4
```

## 样例说明

样例说明一可行方案如下：第二颗棋子向右跳两步，随后第一颗棋子向右跳两步，共 $ 4 $ 步。值得注意的是，第一颗棋子向右跳三步，随后第二颗棋子向右跳一步的方案尽管能把棋子都移动到目标位置，但途中两颗棋子曾经同时在 $ (1, 3) $ ，违反了规则，所以不能选用此方案。

## 数据规模与约定

对于 $100\%$ 的数据，$ n,m \leq 100 $，$ k \leq 500 $。
