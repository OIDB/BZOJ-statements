


## 题目描述
经过跟Farmer John长达数年的谈判，奶牛们终于如愿以偿地得到了想要的旱冰鞋。农场上大部分的区域都很平整，适合在上面滑动，但有一些小块的土地上有很多的岩石，凭奶牛们的旱冰技术，是没有办法通过的。 农场可以看成一个被划分成R(1<=R<=113)行C(1<=C<=77)列的矩阵。快要开饭了，贝茜发现自己在坐标为(1,1)的格子里，并且她想赶到坐标为(R,C)的牛棚去享用她的晚饭。贝茜知道，以她所在的格子为起点，每次向上、下、左、右滑动（但不能沿对角线滑动），一定能找到一条通往牛棚的、不经过任何有大量岩石的格子的路。请你为她指出任意一条通往牛棚的路径。
## 输入格式
* 第1行: 两个用空格隔开的整数，R和C * 第2..R+1行: 每行包含C个字符（不含空格），字符只可能是'.'或'*'。是'.' 的话，表示贝茜能从这个格子里通过，是'*'的话，则这个格子 是不能通过的多岩石地带 
## 输出格式
* 第1..?行: 每行包含2个用空格隔开的整数，表示贝茜回牛棚路径所通过的格 子的坐标。输出的第一行显然应该是1 1，最后一行是R C。输出中 的其余行，依次给出路径中格子的坐标，相邻的两个坐标所表示的 格子必须相邻。 

```input1
5 8
..*...**
*.*.*.**
*...*...
*.*.*.*.
....*.*.

```
```output1
1 1
1 2
2 2
3 2
3 3
3 4
2 4
1 4
1 5
1 6
2 6
3 6
3 7
3 8
4 8
5 8
```

## 提示
没有写明提示
## 题目来源
Gold

