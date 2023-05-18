## 题目描述

Alice 和 Bob 用巧克力棒玩游戏。每次一人可以从盒子里取出若干条巧克力棒，或是将一根取出的巧克力棒吃掉**正整数**长度。

Alice 先手，两人轮流，无法操作的人输。

他们以最佳策略一共进行了 $10$ 轮，请你判断先手必胜或必败。

## 输入格式

共 $10$ 组数据。

每组数据第一行包含一个正整数 $n$，表示巧克力棒条数。

接下来一行 $n$ 个正整数，第 $i$ 个正整数表示第 $i$ 条巧克力棒的长度。

## 输出格式

若先手必胜，请输出 `NO`，反之输出 `YES`（什么奇怪格式）

## 样例

```input1
3
11 10 15
5
13 6 7 15 3
2
15 12
3
9 7 4
2
15 12
4
15 12 11 15
3
2 14 15
3
3 16 6
4
1 4 10 3
5
8 7 7 5 12
```

```output1
YES
NO
YES
YES
YES
NO
YES
YES
YES
NO
```

## 数据范围

$n\le14,1\le a_i\le10^9$