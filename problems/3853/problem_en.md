## Description

Teacher Mai finds that many problems about arithmetic function can be reduced to the following problem:

Maintain an array a with index from $1$ to $l$. There are two kinds of operations:

- Add $v$ to $ax$ for every $x$ that $gcd(x,n)=d$.
- Query Sigma ($X_i$) $(i \le 1 \le X)$

## Input

There are multiple test cases, terminated by a line "0 0".

For each test case, the first line contains two integers $l$ , $Q$ $(1 \le l,Q \le 5*10^4)$, indicating the length of the array and the number of the operations.

In following Q lines, each line indicates an operation, and the format is "$1$ $n$ $d$ $v$" or "$2$ $x$" $(1 \le n,d,v \le 2*10^5,1 \le x \le l)$.

## Output

For each case, output "Case #k:" first, where $k$ is the case number counting from $1$.

Then output the answer to each query.

```input1
6 4
1 4 1 2
2 5
1 3 3 3
2 3
0 0
```

```output1
Case #1:
6
7
```

