## 题目描述

Arietta 的命运与她的妹妹不同，在她的妹妹已经走进学院的时候，她仍然留在山村中。但是她从未停止过和恋人 Velding 的书信往来。一天，她准备去探访他。对着窗外的阳光，临行前她再次弹起了琴。她的琴的发声十分特殊。让我们给一个形式化的定义吧。

所有的 $n$ 个音符形成一棵由音符 $C$（$1$ 号节点）构成的有根树，每一个音符有一个音高 $H_i$。Arietta 有 $m$ 个力度，第 $i$ 个力度能弹出 $D_i$ 节点的子树中，音高在 $[Li,Ri]$ 中的任意一个音符。为了乐曲的和谐，Arietta 最多会弹奏第 $i$ 个力度 $T_i$ 次。

Arietta 想知道她最多能弹出多少个音符。

## 输入格式

输入共 $m+3$ 行。
第一行两个整数 $n,m$，意义如题目所述。
第二行 $n-1$ 个整数 $P_i$ ,表示节点 $i$（$i=2...n$）的父亲节点的编号。
第三行 $n$ 个整数 $H_i$。
接下来的 $m$ 行，每行四个整数 $L_i,R_i,D,T_i$

## 输出格式

输出一个整数表示 Arietta 最多能弹奏多少音符。

```input1
5 2
1 1 2 2
5 3 2 4 1
1 3 2 1
3 5 1 4
```

```output1
4
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n,m\le 10000,1\le H_i,T_i,P_i\le n,1\le L_i\le R_i\le n$。

## 提示

第一个力度弹奏音符 $5$，第二个力度弹奏音符 $1,2,4$。

## 题目来源

Shinrein祭 #1
