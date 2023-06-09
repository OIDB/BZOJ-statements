## 题目描述
Alice 和 Bob 正在玩一个非常无聊的游戏以打发时间。游戏是这样的。初始的时候，有 $n$ 个箱子和 $m$ 个物品。箱子、物品都是不同的。因此有 $n$  $m$ 种方法把这些物品放到箱子里。两个人轮流操作。每一次操作，游戏者有两种选择：添加一个新的箱子或者添加一个新的物品。不可以不操作。如果某人操作以后，将物品放入箱子的方法数大于或等于 $c$ ，那么这个人就输了。保证最初 $c  >  nm$ 。对于一组给定的 $n$ 和 $m$ ，假设游戏者足够聪明，请问是先手必胜，还是后手必胜，还是平局（即无人能获胜）呢？注意，输入文件包含多组测试数据。
## 输入格式
第一行包含一个整数 $T$，表示有 $T$ 组测试数据。
接下来 $T$ 行，每行包含三个整数 $n,m,c$ 。
## 输出格式
输出 $T$ 行，依次表示每组测试数据的答案。若先手必胜输出 `Alice`，后手必胜输出 `Bob`，平局输出 `Draw`。
## 样例输入
```plain
4
2 2 10
5 5 16808
3 1 4
1 4 10
```
## 样例输出
```plain
Alice
Alice
Bob
Draw
```
## 数据范围与约定
对于 $100\%$ 的数据，
$1\le  n  <  c$ ，$1\le  m \le 30$，$2\le  c \le 10^9$，$1\le T\le 5$。