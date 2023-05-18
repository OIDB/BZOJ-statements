


## 题目描述
## 输入格式
    第1行：四个用空格隔开的整数Pj Bi，B2，R. P(1≤P≤5)表示石子的个数，Bi(-5×100000≤Bi≤5×100000)和B2（-5×100000≤B2≤5×100000）表示两个河堤的z坐标，R(1≤R≤5×100000)表示你要描述湖面多少秒．没有两个石子会在同一时间砸到同一地点，两个河堤一定有不同的坐标，没有石子会砸到河堤上去．
    第2到P+1行：每行有三个用空格隔开的整数描述了一颗石子，X，K T(-5×100000≤X，K T≤5×100000).X．y表示石子砸的地点的坐标，T表示石子是什么时候砸下去的．
## 输出格式
    输出是一个9半9的矩阵，中心在(0，0)点．左下点的坐标为(-4，-4)，右上点的坐标为(4，4)．这个矩阵表现的是R秒时湖面状态．

```input1
2 4 100 4
-3 0 1
0 0 2

```
```output1
--------X
-*------X
*-*-*---X
-o-*-*--X
o-----*-X
-o-*-*--X
*-*-*---X
-*------X
--------X
```

## 提示
没有写明提示
## 题目来源
Silver

