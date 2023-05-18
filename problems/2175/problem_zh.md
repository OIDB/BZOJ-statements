## 题目描述

欧洲杯将至，欧足联在欧洲杯之前宣布了一项决定：成立一个新的联赛——欧洲超级联赛，并将欧洲各豪门俱乐部加入该联赛。

众所周知，各联赛都将转播权卖给各电视台以盈利，欧洲超级联赛自然也不例外，可是问题也随之出现：不同的比赛激烈程度自然不同，例如 国际米兰 与 尤文图斯，曼联 与 阿森纳，巴萨罗那 与 皇家马德里 这样的比赛自然人人都愿意看，可是遇上了 利物浦 与 切尔西 这样的比赛球迷们就不高兴啦（至少作者会不高兴）。

因此欧足联为每场比赛定了一个级别,以此来表示比赛的受欢迎程度。

然而，分级的方法却不只一种。例如，可以将所有比赛分为 `A`，`B`，`C` 共 $3$ 种级别，也可以分成 `W`（Wildness，野蛮型），`T`（Technic，技术型）共 $2$ 种级别。

可是如果某轮联赛有多种级别的比赛，精明的电视台当然都会购买最激烈的比赛的转播权，这是欧足联的高官们所不愿看到的（因为联赛的盈利会因此减少），所以每轮联赛只能有同一种级别的比赛。

可挑剔的球迷希望：联赛不是循环的（即无法将联赛分为 $k$（$k$ 为小于 $n$ 的任意正整数）段并使这 $k$ 段都相同），因为这样才不会引起他们的审美疲劳。

已知联赛共有 $n$ 轮，第 $i$ 种分级方法有 $r_i$ 种级别的比赛，现在欧足联想知道在每种分级方法下有多少种安排联赛的方案（注：把某种方案顺移 $k(k\leq n)$ 位后任然是同一种方案，例如，`ABC` 和 `BCA`，`CAB` 为同一种方案，但 `ABC` 和 `ACB` 不是同一种方案）。为此，欧足联设下了奖品，谁能提供答案谁就能获得这份奖励。

## 输入格式

第一行两个数 $n,m$ 分别表示有 $n$ 轮联赛和 $m$ 种分级方法。

第二行 $m$ 个数，第 $i$ 个数为 $r_i$，意义如题。

## 输出格式

$m$ 行，每行一个数 $ans_i$ 表示第 $i$ 种分级方法下的方案数。

## 样例输入

```plain
3 1
3
```

## 样例输出

```plain
8
```

## 样例说明

在样例中，$8$ 种方案分别为 `AAB`，`AAC`，`BBA`，`BBC`，`CCA`，`CCB`，`ABC`，`ACB`。

## 数据规模与约定

对于 $20\%$ 的数据，满足 $m\leq 10$。

对于所有的数据，满足 $n\leq 10^3$，$m\leq 100$，$\forall 1\leq i\leq m,r_i\leq 256$。
