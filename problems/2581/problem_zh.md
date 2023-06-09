## 题目描述

 Farmer John and Bessie have devised a new exercise game for the cows. The cows are running on a circular track of length $M$ ( $2 \le M \le 1,000,000,000$ ) starting from the same position. The game proceeds in $N$ ( $1 \le N \le 14$ ) rounds using a deck of 8N cards each with a number $X_i$ ( $0 \le X_i < M$ ) written on it. Each round FJ moves the top $8$ cards into a separate pile and selects either the top $4$ or bottom $4$ cards for Bessie to play with. Bessie then chooses either the top $2$ cards or bottom $2$ cards of the $4$ cards FJ selected. After this FJ calls out the number on the top card, $X_{top}$, and the cows run a distance of $R * X_{top}$ , where $R$  is the total distance the cows have run so far. Bessie then calls out the number on the bottom card, $X_bottom$ , and the cows run a distance of $X_bottom$ . FJ is concerned that after the exercise the cows will be too tired to get back to the beginning of the track if they end up too far away. He believes if the cows end up more than a distance of K ( $0 \le K \le floor(M/2)$) from their starting position they won't be able to get back home. It is guaranteed that if FJ plays correctly, he will always be able to ensure the cows can come home, irrespective of the moves made by Bessie! For each round, your task is to determine which half of the cards FJ should choose such that no matter what Bessie does from that point on, FJ can always get the cows home. Bessie will then make the move provided in the input and you can then continue onto the next round. Note that even though Bessie's moves are provided to you in the input, you are to specify moves for FJ that would have worked no matter what Bessie chooses (so it is effectively as if FJ does not really know what Bessie will do during her moves). 

题意简述:FJ与Bessie进行 $n$ 轮决策，每轮开始时FJ依次取出 $8$ 张牌，选择前 $4$ 张或后 $4$ 张给bessie，bessie从中选前 $2$ 张或后 $2$ 张，最后得到 $2$ 张牌 $a$ 和 $b$ ，然后其余的奶牛绕长为 $m$ 的圈跑 $dis*a+b$的距离(dis为累计已跑距离)，要求 $n$ 轮过后奶牛离起点的距离不能超过 $k$ 。要求求出FJ的必胜策略（虽已给出bessie的决策方案，但不可用）

## 输入格式

Line 1: Three space-separated integers N, M, K

Line 2: A string N characters. If the ith character is 'T' it means Bessie will select the top 2 cards in the ith round. Otherwise the ith character will be 'B' to indicate Bessie will select the bottom 2 cards in the ith round.
*** Lines 3..2+N: Each line contains eight integers representing the 8 cards to be used that round from top to bottom. **

## 输出格式

 Line 1: A string of N characters where the ith character is 'T' if FJ should choose the top 4 cards or 'B' if FJ should choose the bottom 4 cards in the ith round. If there are multiple ways to get the cows home, choose the lexicographically first (that is, the string that is alphabetically smallest).

```input12 2 0
TT
1 0 0 0 0 0 0 1
0 1 1 1 0 0 1 0
```

```output1TB

```

## 提示

没有写明提示

## 题目来源

没有写明来源

