## Description

The railway network of the Byteotian Railways (BR) consists of bidirectional tracks connecting certain pairs of stations. Each pair of stations is connected by at most one segment of tracks. Furthermore, there is a unique route from every station to every other station. (The route may consist of several segments of tracks, but it may not pass through any station more than once.) 

Byteasar is an undercover inspector of the BR. His job is to pick one of the stations (denote it by $S$) for centre of his operations and to travel to all other stations. His journey should be as follows:

- Byteasar starts in station $S$.

- Next, he picks one of the stations he did not yet control and goes to it along the shortest path (by train, of course), inspects the station, and then goes back to $S$.

- The crooked employees of BR warn one another of Byteasar's comings. To deceive them, Byteasar picks the next station for control in such a way that he sets off from the station Sin different direction than the last time, i.e., along a different segment of tracks leaving from $S$.

- Each station (except $S$) is inspected exactly once.

- After inspecting the last station Byteasar does not come back to $S$.

The travel time along every segment of tracks takes the same amount of time: one hour.

Byteasar intends to consider all the stations as the initial station $S$. For each of them he wants to know the order of inspecting the remaining stations that minimises the total travel time, provided that it is possible at all for that particular $S$.

## Input

The first line of the standard input contains a single integer $N$ that denotes the number of stations. These are numbered from $1$ to $N$. The following $N-1$ lines specify the track segments, one per line. Each of them holds two integers $a,\ b$, separated by a single space, indicating that there is a track segment connecting the stations $a$ and $b$. Each track segments appears exactly once in the description. 

## Output

Your program should print lines on the standard output, each holding a single integer. The one in the $i$-th line should be the minimum number of hours Byteasar has to spend travelling to inspect the stations when $S=i$ if inspecting them all is possible for $S=i$; if it is not, the i-th line should hold the number $-1$. 

```input1
9
3 6
2 4
2 6
2 5
1 7
2 7
8 9
7 8
```

```output1
-1
23
-1
-1
-1
-1
-1
-1
-1
```

## Constraints

For $30\%$ data, $1\leq n\leq 2\times 10^3$.

For $100\%$ data, $1\leq n\leq 10^6$, $1\leq A,\ B\leq N$.

## Source

Acknowledge Object022.