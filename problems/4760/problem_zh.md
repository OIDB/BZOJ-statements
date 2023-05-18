## 题目描述

你可能玩过石头剪刀布这个游戏，奶牛们也喜欢玩类似的游戏，叫做“蹄子剪刀布”。

蹄子剪刀布的规则和石头剪刀布的规则是一样的，蹄子踩碎剪刀，剪刀剪布，布包蹄子。

现在 FJ 想要和他的最机智的奶牛 Bessie 玩蹄子剪刀布（我也不知道 FJ 为什么有蹄子），一共进行了 $n$ 轮，Bessie，作为一个奶牛，非常的怠惰，无论她出什么，都喜欢连续的出，最多变化 $k$ 次，也就是说，对于她所出的，记为序列 $f(i)$，记 $sum$ 为有多少个 $i$ 满足 $f(i)\neq f(i-1)$（$i>1$），而她的 $sum$ 一定不会超过 $k$。

现在 FJ 已经给出了他出的东西，你要告诉 Bessie，在不确定她出的东西的情况下，她最多能赢多少次。

## 输入格式

输入数据第一行为 $n,k$。

接下来 $n$ 行表示 FJ 所出的东西，`H` 表示 hoof，`P` 表示 paper，`S` 表示 Scissors。

## 输出格式

输出在变化不超过 $k$ 次的前提下，最多能赢多少次。

```input1
5 1
P
P
H
P
S
```
```output1
4
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n \le 10^5$，$0\le k \le 20$。

## 题目来源

Gold