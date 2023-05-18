## 题目描述

没头脑和不高兴是一对形影不离的好朋友，他们一起上学也一起玩耍。这天，这对好朋友聚在一起玩纸牌游戏。他们所玩的纸牌总共有 $n$ 张，每一张上面都有一个 $1 \sim n$ 的数字，任意两张纸牌上的数字都不相同。根据他们制定的游戏规则，在每局游戏的开始，所有的牌需要按照从 $1 \sim n$ 的顺序排好。在开心地玩完了一局牌之后，他们发现牌的顺序被弄得乱七八糟，将它们排好序是一件挺麻烦的事情。他们将凌乱的纸牌在桌面上排成一排，然后开始了排序工作。不高兴由于在上一局游戏中输了牌，非常不高兴。他只将其中**奇数位置**的牌排成了升序，然后把剩下的任务推给了没头脑。没头脑非常没头脑，他采取了一个有些笨的排序方式。每次，他找到两张相邻并且顺序不对的牌交换它们，直到整个序列被排好序为止。乐于探究的你，想要研究在初始排列随机的情况下没头脑花在交换纸牌上的时间。假设没头脑每交换一对纸牌花费的时间为  $1$，你希望求出他排序时间的期望。此外，为了更好地分析这个问题，你还希望能够计算出所花时间的方差。更进一步地，如果**被不高兴排好序的位置发生了变化**，你是否还能求出没头脑用来排序时间的期望呢？

## 输入格式

- 输入文件共 $m+1$ 行。
- 第一行包含两个正整数 $n,m$。
- 接下来 $m$ 行，每行包含三个整数 $l$,$r$,$v$。其中 $1 \le l \le r \le n$，$v\in\{0,1\}$。若 $v=0$ 则表示不高兴不再对 $l$ 到 $r$ 之间的位置排序；反之若 $v=1$ 则表示被不高兴排序的位置将涵盖 $l$ 到 $r$。

## 输出格式

- 输出文件共 $m+2$ 行。每行输出一个形如  `p/q`  的有理数，其中 $\gcd(p,q)=1$，$q \ne 1$，$p,q \in \Z$。
- 第一行输出在初始条件下没头脑排序时间的期望。
- 第二行输出在初始条件下没头脑排序时间的方差。
- 接下来 $m$ 行，每行分别输出在对不高兴排序的位置进行了前若干次修改之后没头脑排序时间的期望。



```input1
3 3
2 3 0
2 2 1
1 3 1
```



```output1
2/3
2/9
3/2
1/1
0/1
```

## 样例说明

在初始条件下，不高兴会将位置 $1$ 和 $3$ 的纸牌排好顺序。对于排列 $(1,2,3)$ 和 $(3,2,1)$，他将排列成  $(1,2,3)$，没头脑不需要操作；对于排列 $(1,3,2)$ 和  $(2,3,1)$，他将排列成 $(1,3,2)$ ，没头脑需要交换一次；对于排列 $(2,1,3)$ 和 $(3,1,2)$，他将排列成  $(2,1,3)$，没头脑需要交换一次。因此没头脑所花的时间期望为 $\frac{0 \times 2+1 \times 2+1\times 2}{6}=\frac{2}{3}$；方差为 $\frac{ (0-\frac{2}{3})^2 \times 2 + (1-\frac{2}{3})^2 \times 2+(1-\frac{2}{3})^2 \times 2 }{6}=\frac{2}{9}$。在进行了第一次修改之后，不高兴会只对位置 $1$ 排序，这和没有排序的效果一样；第二次修改之后，他会对位置 $1,2$ 排序；最后一次修改之后，他会对位置 $1,2,3$ 排序，这样没头脑完全不用参与排序工作。可据此求出对应情况下没头脑排序时间的期望。

## 数据规模和约定

对于 $100\%$ 的数据，$1 \le n,m \le 10^5$。
