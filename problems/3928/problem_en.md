## Background

The aliens from outer space have (finally!) invaded Earth. Defend yourself, or be disintegrated! Or assimilated. Or eaten. We are not yet sure.

## Descriptions

The aliens follow a known attack pattern. There are $n$ attackers, the $i$-th one appears at time $a_i$, at distance $d_i$ from you. He must be destroyed no later than at time $b_i$, or else he will fire his weapon, which will definitely end the fight. 

Your weapon is an area-blaster, which can be set to any given power. If fired with power $R$, it momentarily destroys all aliens at distance $R$ or smaller. It also consumes $R$ fuel cells. Determine the minimal cost (measured in fuel cells) of destroying all the aliens, without being killed.

## Input Format

The first line of input contains the number of test cases $T$. The descriptions of the test cases follow:

Each test case starts with a line containing the number of aliens $n$. Of the next $n$ lines, the $i$-th one contains three integers $a_i,b_i,d_i$ .  
The $i$-th alien appears at time $a_i$, is idle until $b_i$, and his distance from you is $d_i$.

## Output Format

For each test case, output one line containing the minimum number of cells needed to destroy all the aliens.

```input1
1
3
1 4 4
4 7 5
3 4 7
```

```output1
7
```

## Limit and hint

For $100\%$ of testcases, $1\le T\le 250$, $1\le n\le 300$, $1\le a_i< b_i\le 10^4$, $1\le d_i\le 10^4$.

## Source

[ACM ICPC 2014-2015 Central European Regional Contest, Problem L](https://cerc.tcs.uj.edu.pl/2014/data/l.pdf)

