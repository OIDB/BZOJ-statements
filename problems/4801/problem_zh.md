## 题目描述

小 $Q$ 同学正在和糖老师一起打（d）牌（p）。这个游戏需要 $52$ 张牌，分为四种花色（`H` 表示红心，`S` 表示黑桃，`C` 表示梅花 ，`D` 表示方块），每种花色有 `A,K,Q,J,10,9,8,7,6,5,4,3,2` 这么多张牌，其中 `A` 是最大的，`2` 是最小的。

游戏的第一轮从小 Q 同学开始，他会先展示一张牌，然后轮到糖老师展示一张牌。双方都展示完手牌之后进入结算环节， 展示较大的牌的人会获得这一轮的胜利（如果两个人展示的牌大小相同那么先展示牌的人获胜），并且得到较大的牌对应的分值，分值就是牌上的数字，比如 `J` 是 $11$，`Q` 是 $12$，`K`是 $13$，`A` 是 $1$。结算后扔掉这一轮展示的牌，然后从上一轮 的获胜者开始下一轮，游戏进行到双方打完所有牌为止。

为了简单起见，现在每个人都只有两张牌，并且全过程中双方都能看到对方的手牌，也就是明牌打。你需要求出两个人都使用最优策略的情况下，小 Q 同学的得分减去糖老师的得分的最大值。

## 输入格式

第一行是一个正整数 $T$，表示测试数据的组数。

每组测试数据包含两行，每行有两张牌，分别表示小 Q 和糖老师手上的牌。每张牌会按照 `XY` 的格式给出，其中 `X` 是 `A,K,Q,J,T(表示10),9,8,7,6,5,4,3,2` 之一， `Y` 是花色（`H,S,C,D` 之一）。保证任何一张牌至多出现一次。

## 输出格式

对于每组测试数据，输出一个整数，表示结果。

## 样例输入

```plain
2
AH 2S
3C 4D
2H 5S
3C 4D
```

## 样例输出

```plain
-3 
1
```

## 数据范围与约定

对于 $100\%$ 的数据，$1\le T \le 10^4$。

## 题目来源

鸣谢 Tangjz 提供试题

