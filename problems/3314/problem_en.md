## Description

Farmer John's $N$ cows are grazing along a one-dimensional fence. Cow i is standing at location $x_i$ and has height $h_i$. 

A cow feels "crowded" if there is another cow at least twice her height within distance $D$ on her left, and also another cow at least twice her height within distance $D$ on her right. Since crowded cows produce less milk, Farmer John would like to count the number of such cows. Please help him. 

## Input

Line $1$: Two integers, $N$ and $D$. 

Lines $2\sim 1+N$: Line $i+1$ contains the integers $x_i$ and $h_i$. The locations of all $N$ cows are distinct.

## Output

Line $1$: The number of crowded cows.

```input1
6 4
10 3
6 2
5 3
9 7
3 6
11 2
```

```output1
2
```

## Sample Explain 1

There are $6$ cows, with a distance threshold of $4$ for feeling crowded. Cow #$1$ lives at position $x=10$ and has height $h=3$, and so on.

The cows at positions $x=5$ and $x=6$ are both crowded. 

## Data scale and Agreement

For $100\%$ data, $1\leq N\leq 5\times 10^4$, $1\leq x_i,h_i,D\leq 10^9$.

## Source

Silver