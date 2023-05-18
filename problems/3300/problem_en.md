## Description
Recently, the cows have been competing with strings of balanced parentheses and comparing them with each other to see who has the best one. 

Such strings are scored as follows (all strings are balanced): 

- the string $\texttt{()}$ has score $1$;
- if $A$ has score $s(A)$ then $\texttt{(}A\texttt{)}$ has score $2\times s(A)$;
- and if $A$ and $B$ have scores $s(A)$ and $s(B)$, respectively, then $AB$ has score $s(A)+s(B)$.

For example, $s(\texttt{(())()})=s(\texttt{(())})+s(\texttt{()})=2\times s(\texttt{()})+1=2\times 1+1=3$. 

Bessie wants to beat all of her fellow cows, so she needs to calculate the score of some strings. Given a string of balanced parentheses of length $N$, help Bessie compute its score. 

## Input
Line $1$: A single integer: $N$;

Lines $2\sim N+1$: Line $i+1$ will contain $1$ integer: $0$ if the $i$-th character of the string is `(`, and $1$ if the ith character of the string is `)`.

## Output

Line $1$: The score of the string. Since this number can get quite large, output the score modulo $12345678910$.

```input1
6
0
0
1
1
0
1
```

```output1
3
```

## Sample Explain 1

This corresponds to the string `(())()`.

## Data scale and Agreement

For $100\%$ data, $2\leq N\leq 10^5$.

## Source

Silver