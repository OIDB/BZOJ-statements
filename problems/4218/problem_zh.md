## 题目描述

n+e 可是不知道比我们高到哪里去了，早在五年前就已经有了一个规模庞大的后宫,而且现在这个后宫还在不断地扩容中......

现在，在 n+e 的后宫中，一共有 $n$ 个妹子，其中,有一些妹子会喜欢（？！）另一个妹子的，这可以用一个亲密度 $L_{x,y}$ 表示（注意这个关系是单向的，而且一个妹子是可以喜欢自己的）。

然而，这些关系里面有一些是不和谐的，比如亲密度过高或者过低都会造成 n+e 后宫的不稳定（为什么过高会造成不稳定呢？我也不知道,你问 n+e 去吧），由于 n+e 参加省队训练去了，没办法自己来稳定后宫，于是他决定更改一些妹子的亲密度（？！），具体来说，他会把某一个妹子变得主动，即所有是「她喜欢别的妹子的关系的亲密度」$L_{x,y}$ 增加 $P_x$，以及将某一个妹子变得不太友好，即所有是「别的妹子喜欢她的关系的亲密度」$L_{x,y}$减少 $Q_y$（每一个操作在同一个妹子身上只会进行一次， 两个操作在同一个妹子身上可以都进行）。

最终，n+e 希望他的后宫中，每一对关系都在一个和谐的范围（即 $[S_{x,y},T_{x,y}]$）内。不过由于 n+e 的妹子也是不知道高到哪里去了，所以她们并不希望自己被变得太主动或者太不友好，也就是说 $P,Q$ 都不可以超过 $10^6$，并且都是非负整数。当然 n+e 希望自己的后宫的妹子们越亲密越好啦，所以他想让你求出他的后宫的最大可行的亲密度总和。（PS：如果你知道怎么弄出合法方案，n+e 说不定会奖励你一个妹子）

一句话题意：

给定一张带权有向图，现在对每个点执行两种操作：将其所有出边权值加上一个数，再将其所有入边权值减去一个数，要求最后每条边权值都在输入的范围以内，请求出操作之后边权和最大是多少。

## 输入格式

**本题有多组数据**。

第一行输入一个正整数 $DataT$，表示 n+e 的后宫数。

接下来 $DataT$ 组数据，每组数据的第一行输入两个正整数 $n,m$，表示 n+e 的这个后宫中的妹子数量以及关系个数。接下来 $m$ 行，每行五个正整数 $(x,y,L,S,T)$，表示妹子 $x$ 喜欢妹子 $y$，初始亲密度为 $L$，修改后上下界分别为 $S,T$。

## 输出格式

对于每组数据，请输出一个整数表示最后的最大亲密度和。若不存在合法方案，请输出 `Unlike`，每组数据占一行。

## 样例
```input1
2
2 4
1 1 2 5 10
1 2 4 8 10
2 1 3 5 10
2 2 2 7 10
2 4
1 1 1 7 7
1 2 7 7 7
2 1 7 7 7
2 2 7 7 7
```
```output1
37
Unlike
```
## 数据规模与约定

对于 $100\%$ 的数据：$0\le L,S,T\le 3\times 10^3$。

保证输入数据中不会有重边。