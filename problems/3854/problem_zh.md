


## 题目描述
Teacher Mai has a kingdom consisting of n cities. He has planned the transportation of the kingdom. Every pair of cities has exactly a one-way road.
He wants develop this kingdom from one city to one city.
Teacher Mai now is considering developing the city w. And he hopes that for every city u he has developed, there is a one-way road from u to w, or there are two one-way roads from u to v, and from v to w, where city v has been developed before.
He gives you the map of the kingdom. Hope you can give a proper order to develop this kingdom.
## 输入格式
There are multiple test cases, terminated by a line "0".
For each test case, the first line contains an integer n (1<=n<=500).
The following are n lines, the i-th line contains a string consisting of n characters. If the j-th characters is 1, there is a one-way road from city i to city j.
Cities are labelled from 1.
## 输出格式
If there is no solution just output "-1". Otherwise output n integers representing the order to develop this kingdom.

```input1
3
011
001
000
0

```

```output1
1 2 3
```

## 提示
请不要提交，期待SPJ
## 题目来源
By 镇海中学


