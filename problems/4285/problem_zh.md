## 题目描述

公元 8192 年，人类进入星际大航海时代。在不懈的努力之下，人类占领了宇宙中的 $n$ 个行星，并在这些行星之间修建了 $n - 1$ 条星际航道，使得任意两个行星之间可以通过唯一的一条路径互相到达。

同时，在宇宙中还有一些空间跳跃点，有些跳跃点已经被发现，还有一些是未知的，每个跳跃点连接了两个行星，使得这两个行星中的任意一个都可以通过这个跳跃点到达另外一个行星。这些跳跃点因为充斥着巨大的能量，所以它们很容易崩溃。

宇宙中还有一些意图毁灭人类的外星人，他们派出了一些使者潜伏在行星上。现在这些使者想要离开他们各自藏身的行星 $u$，到其他行星 $v$ 去搜集情报。由于这些使者十分小心， 他们不会经过任意一条属于这两个行星的路径上的星际航道（即不会走在 $u$ 到 $v$ 路径上的星际航道）。这样他们就只能借助一些跳跃点来到达目的地，但是这些外星人的身体十分脆弱，所以他们只能通过最多一个跳跃点。

现在告诉你若干个按照时间顺序给出的事件，每个事件可能是一个跳跃点又被发现了，也可能是一个跳跃点崩溃了，还有可能是一个外星使者想离开行星 $u$ 到行星 $v$ 去。

请问每个外星使者有多少条不同的路径可以选择？

## 输入格式

第一行一个正整数 $n$。

接下来 $n - 1$ 行每行两个整数 $u, v$，表示一条星际航道连接行星 $u$ 与行星 $v$。

接下来一行一个正整数 $m$，表示已经被发现的跳跃点个数。

接下来 $m$ 行每行两个整数 $s, t$，表示一个跳跃点连接行星 $s$ 与行星 $t$。

接下来一行一个正整数 $q$，表示事件个数。

接下来 $q$ 行每行为以下三种事件中的一种：

`1 x y` ：表示有一个连接行星 $x$ 与行星 $y$ 的跳跃点被发现了；

`2 x y` ：表示有一个连接行星 $x$ 与行星 $y$ 的跳跃点崩溃了（保证存在这样
一个跳跃点） ；

`3 x y` ：表示有一个外星使者想从行星 $x$ 到行星 $y$ 去搜集情报。

## 输出格式

对于每个外星使者输出一行一个整数， 表示这个外星使者可以选择的不同路径条数。

## 样例输入

```plain
13
1 2
1 3
1 4
2 5
5 9
5 10
5 11
10 13
3 6
4 7
4 8
7 12
6
2 4
10 12
9 8
6 7
3 11
7 10
5
1 1 5
3 5 4
2 7 10
2 10 12
3 5 4
```

## 样例输出

```plain
3
1
```

## 提示

对于 $100\%$ 的数据，$n \le 10^5$，$m \le 5 \times 10^4$，$q \le 5 \times 10 ^ 4$，数据保证 $x \ne y$。

数据已加强，By nzhtl1477。2016.9.13。