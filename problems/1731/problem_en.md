## Description

Like everyone else, cows like to stand close to their friends when queuing for feed. FJ has $n \ (2 \le  n \le  10^3)$ cows numbered $1\dots n$ standing along a straight line waiting for feed. The cows are standing in the same order as they are numbered, and since they can be rather pushy, it is possible that two or more cows can line up at exactly the same location (that is, if we think of each cow as being located at some coordinate on a number line, then it is possible for two or more cows to share the same coordinate). Some cows like each other and want to be within a certain distance of each other in line. Some really dislike each other and want to be separated by at least a certain distance. A list of $ml \ (1 \le  ml \le  10^4)$ constraints describes which cows like each other and the maximum distance by which they may be separated;a subsequent list of $md$ constraints $\ (1 \le  md \le  10^4)$ tells which cows dislike each other and the minimum distance by which they must be separated. Your job is to compute, if possible, the maximum possible distance between cow $1$ and cow $n$ that satisfies the distance constraints.

## Input Format

- Line $1$: Three space-separated integers: $n,ml$, and $md$.
- Lines $2 \ldots ml+1$: Each line contains three space-separated positive integers: $a,b$, and $d$, with $1 \le  a < b \le  n$. Cows $a$ and $b$ must be at most $d \ (1 \le  d \le  10^6)$ apart.
- Lines $ml+2 \ldots ml+md+1$: Each line contains three space-separated positive integers: $a,b$, and $d$, with $1 \le  a < b \le  n$. Cows $a$ and $b$ must be at least $d \ (1 \le  d \le  10^6)$ apart.

## Output Format

* Line $1$: A single integer. If no line-up is possible, output `-1`. If cows 1 and N can be arbitrarily far apart, output `-2`.
Otherwise output the greatest possible distance between cows $1$ and $n$.

```input1
4 2 1
1 3 10
2 4 20
2 3 3
```

```output1
27
```

There are $4$ cows. Cows $1$ and $3$ must be no more than $10$ units apart, cows $2$ and $4$ must be no more than $20$ units apart, and cows $2$ and $3$ dislike each other and must be no fewer than $3$ units apart.
