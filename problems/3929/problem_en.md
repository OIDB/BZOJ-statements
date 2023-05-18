## Description

You are given a circular string of length $n$ that consists of digits $\texttt{1..9}$. You want to split it into $k$ continuous non-empty parts. Each of those parts represents a decimal notation of some integer number. Your goal is to find a partition that minimizes the maximum integer from the partition at hand.

For example, if the string is $\texttt{7654321}$ and $k=3$ then the optimal partition is $\{\texttt{176},\texttt{54},\texttt{32}\}$ which has $\texttt{176}$ as the maximum number. Note that the string is cyclic, that is the first character goes right after the last one (as in the $\texttt{176}$ part of the above example).

## Input Format

The first line of the input contains two integers $n$ and $k$.  
The second line contains a string of length $n$ which consists only of characters $\texttt{1..9}$.

## Output Format

Output the value of the maximal number in the optimal partition.


```input1
4 2
4321
```

```output1
32
```

```input2
7 3
7654321
```

```output2
176
```

```input3
5 5
12321
```

```output3
3
```

## Hint

In the first sample the optimal partition is $\{\texttt{32},\texttt{14}\}$.  
In the second sample the optimal partition is $\{\texttt{176},\texttt{54},\texttt{32}\}$.  
In the third sample the optimal (and the only possible) partition is $\{\texttt 1,\texttt 2,\texttt 3,\texttt 2,\texttt 1\}$.

## Limits

For $100\%$ of testcases, $3\le n\le 10^5$, $2\le k\le n$.

## Source

[SouthEastern European Regional Contest 2014, Problem B](http://acm.ro/2014/prob/probleme/B.pdf)