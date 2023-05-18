## 题目描述

Luka 非常擅长解决汉诺塔问题，他发明了一种类似汉诺塔的使用盘子和柱子的游戏。这个游戏有 $n$ 个不同大小的盘子以及 $36$ 根柱子。盘子按照大小从小到大依次被编号为 $1$ 到 $n$。柱子形成了 $6$ 行 $6$ 列的矩阵，从上到下每行依次被编号为 $1$ 到 $6$，从左到右每列依次被编号为 $1$ 到 $6$。

![](file://pic1.jpg)

游戏一开始，$n$ 个盘子都被堆叠在左上角坐标为 $(1,1)$ 的柱子上。对于每一次操作，玩家可以选择一个柱子，取出最顶上若干个盘子，然后选择右边或者下面的某个柱子，将取出的盘子全部堆叠在其顶上（不会翻转顺序）。游戏的目标是把所有盘子都移动到 $(6,6)$，且自底向上大小依次递减。

给定游戏的初始局面，请找到任意一组玩通关的方法。数据保证解必定存在。

## 输入格式

第一行包含一个正整数 $n$，表示盘子的数目。  
第二行包含 $n$ 个正整数 $d_1,d_2,\dots,d_n$，自底向上表示 $(1,1)$ 柱子上每个盘子的编号。  
输入数据保证不存在两个盘子的编号相同。

## 输出格式

输出 $m$ 行，$m$ 表示你的解中游戏操作的次数。  
其中第 $i$ 行包含 $4$ 个参数 $r_i,c_i,p_i,n_i$，表示第 $i$ 步操作，即你选择了 $(r_i,c_i)$ 最上方的 $n_i(n_i\ge 1)$ 个盘子，然后往 $p_i$ 方向移动。  
如果向右移动，那么 $p_i$ 为 `R`；如果向下移动，那么 $p_i$ 为 `D`。  
若有多组方案，输出任意一组。




```input1
6
1 6 5 4 3 2
```


```output1
1 1 D 6
2 1 D 6
3 1 D 6
4 1 D 6
5 1 D 6
6 1 R 6
6 2 R 6
6 3 R 6
6 4 R 6
6 5 R 5
6 5 R 1
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le d_i\le n\le 4\times 10^4$。