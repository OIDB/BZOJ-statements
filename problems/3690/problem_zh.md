## 题目描述

给出一个 $N\times M$ 的方格棋盘，每个格子里有一盏灯和一个开关，开始的时候，所有的灯都是关着的。用 $(x,y)$ 表示第 $x$ 行，$y$ 列的格子。$(x,y)$ 的开关可以改变 $(x,y)$ 中灯的状态，同时也可以改变满足 $|x’-x|=2,|y’-y|=1$ 或者 $|x’-x|=1,|y’-y|=2$ 的格子 $(x’, y’)$ 的状态。改变状态的意思是，原来开着的灯会被关掉，原来关着的灯会被开起来。注意这边的改变状态是强制改变的。每个格子的开关最多只能按一次，求能使得所有灯都打开的方案数$\mod 123456789$的值。

## 输入格式

一行，$N,M$。

## 输出格式

输出一个整数，表示答案。

```input1
2 3
```

```output1
4
```

## 数据规模与约定

对于 $100\%$ 的数据，$N,M\le 150$。

## 提示

```
XX.    .X.    XXX    .XX
XX.    XXX    .X.    .XX
```

其中`X`代表按这个格子的开关。

