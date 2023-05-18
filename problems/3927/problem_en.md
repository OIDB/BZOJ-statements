## Description

Son Halo owns $n$ spaceships numbered from $1$ to $n$ and a space station. They are initially placed on one line with the space station so the spaceship $i$ is positioned $x_i$ meters from the station and all ships are on the same side from the station $(x_i>0)$. All $x_i$ are distinct. Station is considered to have number $0$ and $x_0$ is considered to be equal to $0$.

Every two spaceships with consequent numbers are connected by a rope, and the first one is connected to the station. The rope number $i$ (for $1\le i\le n$) connects ships $i$ and $i-1$. Note, that the rope number $1$ connects the first ship to the station.

Son Halo considers that the rope $i$ and the rope $j$ intersect when the segments $[x_i^{\min},x_i^{\max}]$ and $[x_j^{\min},x_j^{\max}]$ have common internal point but neither one of them is completely contained in the other, where $x_k^{\min}=\min\{x_{k-1},x_k\},x_k^{\max}=\max\{x_{k-1},x_k\}$. That is:
$$
\begin{cases}
x_i^{\min}< x_j^{\min}\land x_j^{\min}< x_i^{\max}\land x_i^{\max}< x_j^{\max}\\
x_j^{\min}< x_i^{\min}\land x_i^{\min}< x_j^{\max}\land x_j^{\max}< x_i^{\max}
\end{cases}
$$
Son Halo wants to rearrange spaceships in such a way, that there are no rope intersections. Because he is lazy, he wants to rearrange the ships in such a way, that the total number of ships that remain at their original position $x_i$ is maximal. However, ships can occupy any real positions $x_i$ after rearrangement.

Your task is to figure out what is the maximal number of ships that can remain at their initial positions.

## Input Format

The first line of the input file contains $n$ - the number of ships. The following line contains $n$ distinct integers $x_i$ - the initial positions of the spaceships.

## Output Format

The output file must contain one integer - the maximal number of ships that can remain at their initial positions in the solution of this problem.

```input1
4
1 3 2 4
```

```output1
3
```

```input2
4
1 4 2 3
```

```output2
4
```

## Limit and Hint

For $100\%$ of testcases, $1\le n\le 2\times 10^5$, $1\le x_i\le n$. 

In the first sample Son Halo can remove the second spaceship in the position between the first and the third to solve the problem while keeping $3$ other ships at their initial positions.  
In the second sample there are no rope intersections, so all $4$ ships can be left at their initial positions.

## Source

[ACM ICPC 2014-2015, NorthEastern European Regional Contest](https://neerc.ifmo.ru/archive/2014/neerc-2014-statements.pdf), Problem I