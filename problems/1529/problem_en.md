## Statement

Byteazar the Dragon has $N$ piggy banks. Each piggy bank can either be opened with its corresponding key or smashed. Byteazar has put the keys in some of the piggy banks - he remembers which key has been placed in which piggy bank. Byteazar intends to buy a car and needs to gain access to all of the piggy banks. However, he wants to destroy as few of them as possible. Help Byteazar to determine how many piggy banks have to be smashed.

TaskWrite a programme which:

reads from the standard input the number of piggy banks and the deployment of their corresponding keys,finds the minimal number of piggy banks to be smashed in order to gain access to all of them,writes the outcome to the standard output.

## Input Format

The first line of the standard input contains a single integer $N$ ($1\le N\le 10^6$) - this is the number of piggy banks owned by the dragon. The piggy banks (as well as their corresponding keys) are numbered from $1$ to $N$. Next, there are $N$ lines: the $(i+1)$'st line contains a single integer - the number of the piggy bank in which the $i$'th key has been placed.

## Output Format

The first and only line of the standard output should contain a single integer - the minimal number of piggy banks to be smashed in order to gain access to all of the piggy banks.

```input1
4
2
1
2
4
```
```output1
2
```

## Constraints

$1 \le N \le 10^6$