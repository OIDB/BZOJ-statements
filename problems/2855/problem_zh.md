## 题目描述

你需要玩一局抽牌的游戏。

一局游戏的参数有 $m,n,a,b,c,id$，这些参数的意义将在下面解释。

游戏里共 $n+m$ 张牌，每张牌唯一的属性是 $0$ 或 $1$，其中有 $n$ 张牌的属性是 $0$，$m$ 张牌的属性是 $1$。

游戏开始前，这些牌会被随机排列。你每一轮可以摸牌顶的 $a$ 张牌，如果这 $a$ 张牌里有不小于 $c$ 张牌的属性是 $1$，那么可以得 $1$ 分，否则不得分；得分判定完成后，这 $a$ 张牌会 **被弃掉**。当牌堆里剩余不足 $a$ 张牌时，游戏结束。

显然，如果你在一开始就知道每个位置的牌的属性，就可以计算出自己的得分，为了使自己的得分尽可能大，还有一个特殊的规则，这部分的规则有两类，由 $id\in\{1,2\}$ 来决定。

当 $id=1$，你可以在每次 **摸到牌顶的 $a$ 张牌后** 立即决定，是正常计算得分并继续游戏，或是 **把摸到的 $a$ 张牌放回牌堆并把剩余的牌重新随机排列**，选择后者的次数 **不能超过** $b$；

当 $id=2$，你可以在 **游戏开始前** 看到每个位置的牌的属性，并立即决定，是按照当前排列进行游戏，或是 **重新随机排列所有的牌** 并重复这个过程，同样的，选择后者的次数 **不能超过** $b$。

需要注意的是，你的所有操作都是为了最大化你得分的期望值。

我们也希望你自己算出在最优操作下的得分的期望值。

## 输入格式

第一行一个整数 $T$ 表示数据组数。

接下来 $T$ 行，每行六个整数 $m,n,a,b,c,id$ 表示一组数据，参数意义见题目描述。

## 输出格式

共 $T$ 行，对于每组数据输出一行一个实数表示你在最优操作下的得分期望值，保留 $6$ 位小数。

```input1
2
5 4 3 4 9 4
2 2 2 1 1 1
```

```output1
1.994791
1.888889
```

## 数据规模与约定

对于 $40\%$ 的数据，满足 $id=1$，在这部分数据中：

- 存在 $10\%$ 的数据，$n,m\leq 5$，$b\leq 10$；
- 存在 $30\%$ 的数据，$b\leq 20$。

对于 $40\%$ 的数据，满足 $id=2$，在这部分数据中：

- 存在 $10\%$ 的数据，$b\leq 10$；

对于 $100\%$ 的数据，$1\leq T\leq 10^3$，$id\in\{1,2\}$，$1\leq n,m\leq 12$，$0\leq b\leq 10^9$，$1\leq a\leq n+m$，$c\ge 0$。