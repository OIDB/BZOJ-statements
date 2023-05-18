## Description

Farmer John is at the market to purchase supplies for his farm. He has in his pocket $K$ coins. FJ would like to make a sequence of $N$ purchases, where the ith purchase costs $c_i$ units of money. As he makes this sequence of purchases, he can periodically stop and pay, with a single coin, for all the purchases made since his last payment (of course, the single coin he uses must be large enough to pay for all of these). Unfortunately, the vendors at the market are completely out of change, so whenever FJ uses a coin that is larger than the amount of money he owes, he sadly receives no changes in return!

Please compute the maximum amount of money FJ can end up with after making his $N$ purchases in sequence. Output $-1$ if it is impossible for FJ to make all of his purchases. 

## Input

Line $1$: Two integers, $K,N$.

Lines $2\sim 1+K$: Each line contains the amount of money of one of FJ's coins.

Lines $2+K\sim 1+N+K$: These $N$ lines contain the costs of FJ's intended purchases.

## Output

Line $1$: The maximum amount of money FJ can end up with, or $-1$ if FJ cannot complete all of his purchases.

```input1
3 6
12
15
10
6
3
3
2
3
7
```

```output1
12 
```

## Sample Explain 1

FJ has $3$ coins of values $12,15,10$. He must make purchases in sequence of value $6,3,3,2,3,7$. 

FJ spends his $10$-unit coin on the first two purchases, then the $15$-unit coin on the remaining purchases. This leaves him with the $12$-unit coin. 

## Data scale and Agreement

For $100\%$ data, $1\leq K\leq 16$, $1\leq N\leq 10^5$, the value of each coin in the range $1\sim 10^8$, $1\leq c_i\leq 10^4$.

## Source

Gold