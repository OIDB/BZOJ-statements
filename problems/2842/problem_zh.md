## 题目描述

Ginny 的生日马上就来了。魔法大叔 Herry 准备给他的新妹子一个生日礼物。礼物是由 $N$ 个魔法珠子串成的魔法手镯。每种不同种类的珠子有其独一无二的特性。Herry 的另一个妹子远坂凛指出，有一些指定种类的成对珠子，如果挨在一块会发生化学反应甚至核聚变，因此 Herry 必须非常小心以确保这些珠子不会相邻。Herry 想知道，究竟能有多少不同的手镯，将这个结果 $\bmod 9973$ 并告诉他。注意，若一个手镯能够通过旋转得到另一个手镯，我们将这两个手镯视为相同的。

## 输入格式

输入包含多组数据。第一行一个正整数 $c$，为数据的组数。接下来的数据分为 $c$ 组，每一组的第一行为三个正
整数 $N,M,K$，$N$ 为珠子的数量，$M$ 为珠子的种类数，$K$ 为不能相邻的种类对数，保证$N \bmod 9973 \ne 0$。接下来 $K$ 行每行两个正整数 $i,j$，表示种类 $i$ 的珠子不能和种类 $j$ 的珠子相邻。

## 输出格式

对于每组数据，输出一行，为手镯的数量。

```input1
4
3 2 0
3 2 1
1 2
3 2 2
1 1
1 2
3 2 3
1 1
1 2
2 2
```

```output1
4
2
1
0
```

## 数据规模与约定

$c\le20$。



