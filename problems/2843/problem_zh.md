## 题目描述

不久之前，Mirko 建立了一个旅行社，名叫“极地之梦”。这家旅行社在北极附近购买了 $N$ 座冰岛，并且提供观光服务。当地最受欢迎的当然是帝企鹅了，这些小家伙经常成群结队的游走在各个冰岛之间。Mirko 的旅行社遭受一次重大打击，以至于观光游轮已经不划算了。旅行社将在冰岛之间建造大桥，并用观光巴士来运载游客。
Mirko 希望开发一个电脑程序来管理这些大桥的建造过程，以免有不可预料的错误发生。这些冰岛从 $1$ 到 $N$ 标号。一开始时这些岛屿没有大桥连接，并且所有岛上的帝企鹅数量都是知道的。每座岛上的企鹅数量虽然会有所改变，但是始终在 $[0,1000]$ 之间。你的程序需要处理以下三种命令：

1. `bridge A B`：在 $A$ 与 $B$ 之间建立一座大桥（$A$ 与 $B$ 是不同的岛屿）。由于经费限制，这项命令被接受，当且仅当 $A$ 与 $B$ 不联通。若这项命令被接受，你的程序需要输出 `yes` ，之后会建造这座大桥。否则，你的程序需要输出 `no` 。
2. `penguins A X`：根据可靠消息，岛屿 $A$ 此时的帝企鹅数量变为 $X$。这项命令只是用来提供信息的，你的程序不需要回应。
3. `excursion A B`：一个旅行团希望从 $A$ 出发到 $B$。若 $A$ 与 $B$ 连通，你的程序需要输出这个旅行团一路上所能看到的帝企鹅数量（包括起点 $A$ 与终点 $B$），若不联通，你的程序需要输出 `impossible` 。

## 输入格式

第一行一个正整数 $N$，表示冰岛的数量。

第二行$N$ 个范围 $[0, 1000]$ 的整数，为每座岛屿初始的帝企鹅数量。

第三行一个正整数 $M$，表示命令的数量。接下来 $M$ 行即命令，为题目描述所示。
## 输出格式

对于每个 `bridge` 命令与 `excursion` 命令，输出一行，为题目描述所示。

```input1
5
4 2 4 5 6
10
excursion 1 1
excursion 1 2
bridge 1 2
excursion 1 2
bridge 3 4
bridge 3 5
excursion 4 5
bridge 1 3
excursion 2 4
excursion 2 5
```
```output1
4
impossible
yes
6
yes
yes
15
yes
15
16
```

## 数据规模与约定

$1\le N\le30000,1\le M\le100000$。
