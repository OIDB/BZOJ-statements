## 题目描述

&emsp;&emsp;魔塔是一款很流行的益智类小游戏。在游戏中，你可以控制主人公在魔塔中移动，走到怪兽面前便可以和怪兽来决斗，打败怪兽后可以得到金钱，并可以通过金钱来提高自己的攻击力、防御力、血量，从而变得更强大。

&emsp;&emsp;然而，即便你拥有再高的攻击力、防御力，可以天下无敌，但一扇小小的门就可以阻止你无法前进。在游戏中，有红、黄、蓝三种颜色的门，并对应有红、黄、蓝三种颜色的钥匙。如果你想通过一扇门，需要消耗一把对应颜色的钥匙打开这扇门，如果你没有这种颜色的钥匙，便不能通过。

&emsp;&emsp;现在你得到一款加强版的魔塔游戏：首先，门和钥匙的颜色不再是三种，而是 $n$ 种，定为 $1\sim n$ 号颜色。对于 $i$ 号颜色的钥匙你有 $K_i$ 把。并且之后你不会以任何形式得到任何颜色的钥匙。在你面前有三座 $n$ 层的魔塔   $A,B,C$ 。每座魔塔的入口处和相邻两层之间都会有一扇门。对于每座魔塔，恰好有 $n$ 扇门，并且这 $n$ 扇门的颜色恰好各不相同。其中，$A$ 魔塔中通往第 $i$ 层的门颜色为 $\mathrm{DoorA_i}$。（$\mathrm{DoorB_i}$ 、$\mathrm{DoorCi}$ 的定义与 $\mathrm{DoorA_i}$ 类似）在每座魔塔的每一层都有一定数量的怪兽，但这些怪兽根本打不过强大的你，你可以不费一滴血就秒杀这些怪兽，并得到杀死他们的金钱。我们已经为你统计好，消灭 $A$ 魔塔第 $j$ 层中所有的怪兽，可以得到的金钱数为 $\mathrm{GoldA_i}$。（$\mathrm{GoldB_i}$、$\mathrm{GoldC_i}$ 的定义与 $\mathrm{GoldA_i}$ 类似）现在，就请你来决策，如何运用这些钥匙，能得到最多的金钱，并告诉我们最多能获得多少金钱。

## 输入格式

第一行一个字符（$A\sim F$），表示数据类型（在下面数据规模中有详细介绍）。

第二行一个整数 $m$ ，表示有几组测试数据。

之后给出 $m$ 组数据，对于每组数据有九行：

第一行一个整数 $n$ ，表示魔塔层数。

第二行一个数列 $K_i$。

第三行至第五行，每行一个数列，分别为 $\mathrm{DoorA}$、$\mathrm{DoorB}$、$\mathrm{DoorC}$。

第六行至第八行，每行一个数列，分别为 $\mathrm{GoldA}$、$\mathrm{GoldB}$、$\mathrm{GoldC}$。

第九行为一个空行。

## 输出格式

输出应包含 $m$ 行，每行一个正整数，为最大能获得的金钱数。

```input1
A
2
5
1 2 1 1 2
1 2 3 4 5
2 4 3 5 1
5 4 3 2 1
1 1 1 1 5
1 2 2 3 3
1 2 1 1 1
5
1 2 1 1 2
1 2 3 4 5
2 4 3 5 1
5 4 3 2 1
1 1 1 1 50
1 2 2 3 3
1 2 1 1 1
```

```output1
12
56
```

## 数据规模与约定

对于 $100\%$ 的数据：

$1\le m\le 10$，$1\le n\le 10^5$，$1\le K_i\le2$。

$0\le  \mathrm{GoldA_i}, \mathrm{GoldB_i}, \mathrm{GoldC_i} \le2\times 10^3$。

$\mathrm{DoorA},\mathrm{DoorB},\mathrm{DoorC}$ 为三个 $1\sim n$ 的排列。

数据共分为六类：$A,B,C,D,E,F$，他们分别有各自的特征：

$A$ 类数据占 $10\%$ ，保证 $1\le n\le 100$。

$B$ 类数据占 $10\%$，保证 $1\le n\le10^3$。

$C$ 类数据占 $10\%$，保证 $\mathrm{GoldC}_i=0$，即第三座塔中没有任何金钱。

$D$ 类数据占 $20\%$，保证 $K_i=1$，即每种钥匙你都只有一把。

$E$ 类数据占 $30\%$，保证 $\mathrm{DoorA},\mathrm{DoorB},\mathrm{DoorC}$   三个 $1\sim n$ 的排列为随机产生的数列。

$F$ 类数据占 $20\%$，没有其他特征。

## 样例说明

对于第一个数据：

`1 2 3 4 5`，第一个魔塔不用钥匙，能得到 $0$ 金钱；

`2 4 3 5 1`，第二个魔塔用 $1,2,3,4,5$ 号钥匙，得到 $11$ 金钱；

`5 4 3 2 1`，第三个魔塔用 $5$ 号钥匙，得到 $1$ 金钱；

最多可得到 $12$ 金钱。

---

对于第二个数据：

`1 2 3 4 5`，第一个魔塔用 $1,2,3,4,5$ 号钥匙，能得到 $54$ 金钱；

`2 4 3 5 1`，第二个魔塔用 $2$ 号钥匙，得到 $1$ 金钱；

`5 4 3 2 1`，第三个魔塔用 $5$ 号钥匙，得到 $1$ 金钱；

最多可得到 $56$ 金钱。

