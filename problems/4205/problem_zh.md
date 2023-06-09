## 题目描述

现在有一种卡牌游戏，每张卡牌上有三个属性值：$A,B,C$。把卡牌分为 $X,Y$ 两类，分别有 $n_1,n_2$ 张。

两张卡牌能够配对，当且仅当，存在至多一项属性值使得两张卡牌该项属性值互质，且两张卡牌类别不同。

比如一张 $X$ 类卡牌属性值分别是 $225,233,101$，一张 $Y$ 类卡牌属性值分别为 $115,466,99$ 。那么这两张牌是可以配对的，因为只有 $101$ 和 $99$ 一组属性互质。

游戏的目的是最大化匹配上的卡牌组数，当然每张卡牌只能用一次。

## 输入格式

数据第一行两个数 $n_1,n_2$，空格分割。

接下来 $n_1$ 行，每行三个数，依次表示每张 $X$ 类卡牌的三项属性值。

接下来 $n_2$ 行，每行三个数，依次表示每张 $Y$ 类卡牌的三项属性值。

## 输出格式

输出一个整数：最多能够匹配的数目。

## 样例
```input1
2 2
2 2 2
2 5 5
2 2 5
5 5 5
```
```output1
2
```
## 样例说明

样例中第一张 $X$ 类卡牌和第一张 $Y$ 类卡牌能配对，第二张 $X$ 类卡牌和两张 $Y$ 类卡牌都能配对。所以最佳方案是第一张 $X$ 和第一张 $Y$ 配对，第二张 $X$ 和第二张 $Y$ 配对。

## 数据规模与约定

对于 $100\%$ 的数据：$n_1,n_2\le 3\times 10^4$，属性值为不超过 $200$ 的正整数。

## 提示

请大胆使用渐进复杂度较高的算法！