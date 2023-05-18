## 题目背景

在森林中见过会动的树，在沙漠中见过会动的仙人掌过后，魔法少女 LJJ 已经觉得自己见过世界上的所有稀奇古怪的事情了。

LJJ 感叹道：

「这里真是个迷人的绿色世界，空气清新、淡雅，到处散发着醉人的奶浆味；小猴在枝头悠来荡去，好不自在；各式各样的鲜花争相开放，各种树枝的枝头挂满沉甸甸的野果；鸟儿的歌声婉转动听，小河里飘着落下的花瓣真是人间仙境。」 

SHY 觉得 LJJ 还是太 naive，一天，SHY 带着自己心爱的图找到 LJJ，对 LJJ 说：

「既然你已经见识过动态树，动态仙人掌了，那么今天就来见识一下动态图吧！」

「要支持什么操作？」

「维护一个动态图，支持如下操作！」

「我可以离线吗？」

「可以，每次操作是不加密的。」

「我可以暴力吗？」

「自重。」

LJJ 很郁闷，你能帮帮他吗？

## 题目描述

你需要维护一个动态图，支持如下操作：

1. 新建一个节点，权值为 $x$；
2. 连接两个节点；
3. 将一个节点 $a$ 所属于的联通块内权值小于 $x$ 的所有节点权值变成 $x$；
4. 将一个节点 $a$ 所属于的联通块内权值大于 $x$ 的所有节点权值变成 $x$；
5. 询问一个节点 $a$ 所属于的联通块内的第 $k$ 小的权值是多少；
6. 询问一个节点 $a$ 所属联通块内所有节点权值之积与另一个节点 $b$ 所属联通块内所有节点权值之积的大小，若 $a$ 所属联通块内所有节点权值之积大于 $b$ 所属联通块内所有节点权值之积，输出 $1$，否则为 $0$； 
7. 询问 $a$ 所在联通块内节点的数量；
8. 若两个节点 $a$，$b$ 直接相连，将这条边断开；
9. 若节点 $a$ 存在，将这个点删去。

## 输入格式

第一行一个整数 $m$，表示操作次数，接下来 $m$ 行，每行若干个整数，描述一次操作。

## 输出格式

对每次询问操作，输出其答案。

```input1
11
1 2
1 3
1 4
1 5
1 6
2 1 2
2 2 3
2 3 4
2 4 5
3 2 5
5 3 4
```

```output1
6
```

## 数据范围与约定

$0\le m\le 400000$，所有出现的数均小于 $10^9$。

## 说明

在不影响原题面的基础上，为了增加阅读体验，对题面格式进行了部分优化。