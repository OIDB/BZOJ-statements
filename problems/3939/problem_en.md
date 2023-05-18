## Description

Just like humans enjoy playing the game of Hopscotch, Farmer John&apos;s cows have invented a variant of the game for themselves to play. Being played by clumsy animals weighing nearly a ton, Cow Hopscotch almost always ends in disaster, but this has surprisingly not deterred the cows from attempting to play nearly every afternoon.

The game is played on an $R$ by $C$ grid, where each square is labeled with an integer in the range $1\sim  K$. Cows start in the top-left square and move to the bottom-right square by a sequence of jumps, where a jump is valid if and only if:

1) You are jumping to a square labeled with a different integer than your current square,

2) The square that you are jumping to is at least one row below the current square that you are on, and

3) The square that you are jumping to is at least one column to the right of the current square that you are on.

Please help the cows compute the number of different possible sequences of valid jumps that will take them from the top-left square to the bottom-right square.

## Input Format
The first line contains the integers $R,C$ and $K$.

The next $R$ lines will each contain $C$ integers, each in the range $1\sim K$.

## Output Format
Output the number of different ways one can jump from the top-left square to the bottom-right square, mod $10^9+7$.


```input1
4 4 4 
1 1 1 1 
1 3 2 1 
1 2 4 1 
1 1 1 1
```

```output1
5
```

## Limit and Hint
For $100\%$ of testcases, $2\le R,C\le 750$, $1\le K\le RC$.

## Source 

USACO 2015 February Contest Gold T1