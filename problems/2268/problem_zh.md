## 题目描述

Jonly is writing his first computer game．For the opening scene he wants to have the main character，Wormly，cross Bridgely，the bridge．Wormly is a worm made of $b$ equal circular bubbles and $L$ legs．At all times each leg has to be under one of the bubbles，and under each bubble there can be at most one leg．Bridgely was supposed to be composed of $n$ planks with the width of each plank equal to the diameter of each of Wormly's bubbles．However，some of the planks are missing．

At every moment，Wormly can do exactly one of the following：

* Move one of its legs forward over any number of（possibly missing）planks．After the move，the leg should be on a plank and underneath one of Wormly's bubbles．A leg isn't allowed to overtake other legs．

* Move all of its bubbles forward one plank while its legs remain on the same planks．After the move each leg must still be under one of Wormly's bubbles．

![](file://pic1.png)

Wormly 是一条虫子，它的身体有 $b$ 个球和 $L$ 条腿。任何时候，它的腿总是在某个球的下方，并且每个球下方至多一条腿。

Wormly 想要过桥。这个桥由本来由 $n$ 块板子组成，但有的板子不见了。

每个时刻里，Wormly 可以做这些事：

* 向前移动一个脚到一块板子，要求不能越过前面的腿（图中 `c` ），不能落在消失的板子上（图中 `a` ）；

* 把所有的球向前移动一格，腿不动。移完之后，每条腿必须还在某个球下。

一开始虫在最左的 $b$ 块板子上，腿在最左的 $L$ 块板子上，最后虫在最右的 $b$ 块板子上，腿在最右的 $L$ 块板子上。这个过程最少要多少时间？

## 输入格式

**本题有多组数据**

On the first line a positive integer：the number of test cases，at most $100$．After that per test case：

One line with three integers $L,b,n$ ：the number of legs，the number of bubbles and the length of the bridge respectively．

One line with a string consisting of $n$ characters，either `0` or `1`，describing Bridgely．A one indicates a plank and a zero indicates a missing plank．

$T$：测试数据组数。

$L,b$ and $n$ ：$n$ 位 $01$ 串，`1` 代表有板子。

## 输出格式

Per test case：

One line with an integer：the minimum number of steps it takes Wormly to cross Bridgely．If it is impossible to get across while satisfying the constraints，the line must contain `IMPOSSIBLE` instead．

Figure 1：In this example，the only possible move for the last leg is to position b．（The plank at position a is missing，so the leg cannot move there．To get to position c，the last leg would have to overtake the first leg．）Also，in this example，moving all the bubbles forward is not allowed because Wormly's last leg would end up without a bubble over it．

Now Jonly is wondering how long the animation takes until Wormly reaches the end of Bridgely．Initially Wormly's bubbles are directly above the leftmost $b$ planks of the bridge and its legs are on the leftmost $L$ planks．At the end of the animation Wormly's bubbles have to be directly above the rightmost $b$ planks and its legs have to be on the rightmost $L$ planks．

The left- and right- most $L$ planks of Bridgely are not missing．

**IMPOSSIBLE或者是最小的通过时间。**

```input1
3
1 2 2
11
2 3 5
11011
1 3 5
11011
```

```output1
1
IMPOSSIBLE
5
```

## 样例解释 1

**移动腿** － **移动球** － **移动腿** － **移动球** － **移动腿** $5$ **步**。

## 数据规模与约定

$100\%$ 的数据满足：$T \le 100$，$1 \le L \le b \le n \le 1 \times 10^6$。