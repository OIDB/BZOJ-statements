## Description

Farmer John's new barn consists of a huge circle of $N$ stalls, numbered $0\sim N-1$, with stall $N-1$ being adjacent to stall $0$.

At the end of each day, FJ's cows arrive back at the barn one by one, each with a preferred stall they would like to occupy. However, if a cow's preferred stall is already occupied by another cow, she scans forward sequentially from this stall until she finds the first unoccupied stall, which she then claims. If she scans past stall $N-1$, she continues scanning from stall $0$.

Given the preferred stall of each cow, please determine the smallest index of a stall that remains unoccupied after all the cows have returned to the barn. Notice that the answer to this question does not depend on the order in which the cows return to the barn.

In order to avoid issues with reading huge amounts of input, the input to this problem is specified in a concise format using $K$ lines each of the form: $X\ Y\ A\ B$.

One of these lines specifies the preferred stall for $X\times Y$ total cows: X cows prefer each of the stalls $f(1)\sim f(Y)$, where $f(i)=(A\times i+B)\bmod N$. Do not forget the standard memory limit of $64\text{MB}$ for all problems.

## Input

Line 1: Two space-separated integers: $N,K$.

Lines $2\sim 1+K$: Each line contains integers $X,Y,A,B$, interpreted as above. The total number of cows specified by all these lines will be at most $N-1$. Cows can be added to the same stall by several of these lines.

## Output

Line $1$: The minimum index of an unoccupied stall. 

```input1
10 3
3 2 2 4
2 1 0 1
1 1 1 7 
```

```output1
5 
```

## Sample Explain 1

There are $10$ stalls in the barn, numbered $0\sim 9$. The second line of input states that $3$ cows prefer stall $(2\times 1+4)\bmod 10=6$, and $3$ cows prefer stall $(2\times 2+4)\bmod 10=8$. The third line states that $2$ cows prefer stall $(0\times 1+1)\bmod 10=1$. Line four specifies that $1$ cow prefers stall $(1\times 1+7)\bmod 10=8$ (so a total of $4$ cows prefer this stall).

All stalls will end up occupied except stall $5$.

## Data scale and Agreement

For $100\%$ data, $2\leq N\leq 3\times 10^6$, $1\leq K\leq 10^4$, $0\leq A,B\leq 10^9$.

## Source

Gold