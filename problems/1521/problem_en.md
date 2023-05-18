## Statement

Let us consider a text consisting of n words numbered from 1 to n. We represent any of its decompositions into k lines by a sequence of numbers ($a_1,a\_2,\cdots,a_{k-1}$), such that the words with numbers from $1$ to $a_1$ are in the first line, the words with umbers from $a_1 + 1$ to $a_2$ are in the second line, and so on, and finally, the words with numbers from $a_{k-1} + 1$ to n are in the last, k-th line.

Each word has a certain length (measured in the number of characters). Let $\operatorname{length}(x)$ denote the length of the word no. . Furthermore, every two subsequent words in a line are separated by a space of width of a single character. By length of the line we denote the sum of lengths of the words in this line, increased by the number of spaces between them. Let $\operatorname{line}(w)$ denote the length of the line no.w . I.e., if the line no.w contains the words with numbers from i to j inclusive, its length is:

```cpp
XXXX (1st line)
XXX XX (2nd line)
XXXXX (3rd line)
```

$\operatorname{line}(w)=\operatorname{length}(i)+\cdots+\operatorname{length}(j)+(j-i)$

As an example, let us consider a text consisting of $4$ words of lengths $4$, $3$, $2$ and $5$, respectively, and its decomposition $(1,3)$ into $3$ lines. Then the length of the first line is $4$, second $-6$ , and third $-5$ :

We shall refer to the number

$|\operatorname{line}(1)-\operatorname{line}(2)|+\cdots+|\operatorname{line}(k-1)-\operatorname{line}(k)|$

as the coefficient of aestheticism of a decomposition of the given text into $k$ lines. Particularly, if the decomposition has only one line, its coefficient of aestheticism is $0$.

Needles to say, the smaller the coefficient, the more aesthetical the decomposition. We shall consider only these decompositions that have no line whose length exceeds some constant $m$. Of all such decompositions of a given text into any number of lines we seek the one most aesthetical, i.e. the one with the smallest coefficient of aestheticism. The aforementioned examplary decomposition's coefficient is $3$, and that is exactly the minimum coefficient of aestheticism for $m=6$ and $m=7$.

## Input Format

The first line of the standard input contains the numbers $m$ and $n$, $1\le m\le 10^6$,$1\le n\le 2\ 000$, separated by a single space. The second, last line of the standard input contains $n$ integers, denotingthe lengths of subsequent words, $1\le length(i)\le m$ for $i=1,2,\cdots,n$, separated by single spaces.

## Output Format

The first and only line of the standard output should contain exactly one integer: the minimumcoefficient of aestheticism for those decompositions, whose every line's length does not exceed $m$.

```intput1
6 4
4 3 2 5
```
```output1
3
```