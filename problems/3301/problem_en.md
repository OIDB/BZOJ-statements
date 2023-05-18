## Description

The $N$ cows conveniently numbered $1...N$ are playing yet another one of their crazy games with Farmer John. The cows will arrange themselves in a line and ask Farmer John what their line number is. In return, Farmer John can give them a line number and the cows must rearrange themselves into that line. 

A line number is assigned by numbering all the permutations of the line in lexicographic order. 

Consider this example: 

Farmer John has $5$ cows and gives them the line number of $3$. 
The permutations of the line in ascending lexicographic order: 

$1$st: $\texttt{1 2 3 4 5}$ 

$2$nd: $\texttt{1 2 3 5 4}$

$3$rd: $\texttt{1 2 4 3 5}$ 

Therefore, the cows will line themselves in the cow line $\texttt{1 2 4 3 5}$. 

The cows, in return, line themselves in the configuration $\texttt{1 2 4 3 5}$ and ask Farmer John what their line number is. 

Continuing with the list: 

$4$th: $\texttt{1 2 4 5 3}$ 

$5$th: $\texttt{1 2 5 3 4}$ 

Farmer John can see the answer here is $5$.

Farmer John and the cows would like your help to play their game. 

They have $K$ queries that they need help with. 

Query $i$ has two parts: $C_i$ will be the command, which is either `P` or `Q`. 

- If $C_i$ is `P`, then the second part of the query will be one integer $A_i$, which is a line number. This is Farmer John challenging the cows to line up in the correct cow line. 

- If C_i is `Q`, then the second part of the query will be $N$ distinct integers $B_{i,j}$. This will denote a cow line. These are the cows challenging Farmer John to find their line number. 

## Input

Line $1$: Two space-separated integers: $N$ and $K$. 

Lines $2\sim 2K+1$: Line $2i$ and $2i+1$ will contain a single query. 

Line $2i$ will contain just one character: `Q` if the cows are lining up and asking Farmer John for their line number or `P` if Farmer John gives the cows a line number. 

If the line $2i$ is `Q`, then line $2i+1$ will contain $N$ space-separated integers $B_{i,j}$ which represent the cow line. If the line $2i$ is `P`, then line $2i+1$ will contain a single integer $A_i$ which is the line number to solve for. 

## Output

Lines $1\sim K$: Line $i$ will contain the answer to query $i$.

If line $2i$ of the input was `Q`, then this line will contain a single integer, which is the line number of the cow line in line $2i+1$. 

If line $2i$ of the input was `P`, then this line will contain $N$ space separated integers giving the cow line of the number in line $2i+1$. 

```input1
5 2
P
3
Q
1 2 5 3 4
```

```output1
1 2 4 3 5
5
```

## Data scale and Agreement

For $100\%$ data, $1\leq N\leq 20$, $1\leq K\leq 10^4$, $1\leq A_i\leq N!$, $1\leq B_{i,j}\leq N$.

## Source

Silver