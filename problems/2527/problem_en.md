## Description

Byteotian Interstellar Union (BIU) has recently discovered a new planet in a nearby galaxy. The planet is unsuitable for colonisation due to strange meteor showers, which on the other hand make it an exceptionally interesting object of study.

The member states of BIU have already placed space stations close to the planet's orbit. The stations' goal is to take samples of the rocks flying by. The BIU Commission has partitioned the orbit into msectors, numbered from $1$ to $m$, where the sectors $1$ and mare adjacent. In each sector there is a single space station, belonging to one of the $n$ member states.

Each state has declared a number of meteor samples it intends to gather before the mission ends. Your task is to determine, for each state, when it can stop taking samples, based on the meter shower predictions for the years to come.

## Input

The first line of the standard input gives two integers, $n$ and $m$ ($1\leq n,\ m\leq 3\times 10^5$) separated by a single space, that denote, respectively, the number of BIU member states and the number of sectors the orbit has been partitioned into.

In the second line there are $m$ integers $O_i$ ($1\leq O_i\leq n$) separated by single spaces, that denote the states owning stations in successive sectors.

In the third line there are $n$ integers $P_i$ ($1\leq P_i\leq 10^9$) separated by single spaces, that denote the numbers of meteor samples that the successive states intend to gather.

In the fourth line there is a single integer $k$ ($1\leq k\leq 3\times 10^5$) that denotes the number of meteor showers predictions. The following $k$ lines specify the (predicted) meteor showers chronologically. The $i$-th of these lines holds three integers $L_i,\ R_i,\ A_i$ (separated by single spaces), which denote that a meteor shower is expected in sectors $L_i,\ L_{i+1},\ \cdots,\ R_i$ (if $L_i\leq R_i$) or sectors $L_i,\ L_{i+1},\ \cdots,\ m,\ 1,\ \cdots,\ R_i$ (if $L_i > R_i$), which should provide each station in those sectors with Aimeteor samples ($1\leq Ai < 10^9$).

In tests worth at least $20\%$ of the points it additionally holds that.

## Output

Your program should print $n$ lines on the standard output. The $i$-th of them should contain a single integer $W_i$, denoting the number of shower after which the stations belonging to the $i$-th state are expected to gather at least $P_i$ samples, or the word `NIE` (Polish for no) if that state is not expected to gather enough samples in the foreseeable future. 

```input1
3 5
1 3 2 1 3
10 5 7
3
4 2 4
1 3 1
3 5 2
```

```output1
3
NIE
1
```

## Source

Thank you Object022.