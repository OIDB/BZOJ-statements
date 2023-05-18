


## 题目描述
超立方体是立方体在高维空间内的拓展（其在 2 维情况下退化为正方形，1
维情况下退化成线段）。在理论计算机科学领域里，超立方体往往可以和 2 进制
编码联系到一起。对理论计算机科学颇有研究的 Will 自然也会对超立方体有着
自己的思考。 
上图就是在 0～4 维空间内超立方体所对应的图形。显然我们可以把超立方
体的每个顶点看成一个点，每一条棱看成一条边，这样就会得到一个无向图，我
们称之为超立方图。 
D维空间内的超立方图有 2D个点，我们把这些点从0到2D-1依次编号。 
有一个有趣而重要的充要结论是：一定存在一种编号的方式，使得图中任意
两个有边相连的顶点的编号的 2进制码中，恰好有一位不同。 
在 2维和3维空间内这个结论可以这样形象的理解： 
对于 2维空间，我们只要把这个正方形放到第一象限内，使得 4个顶点的坐
标按逆时针顺序依次为(0,0)，(1,0)，(1,1)，(0,1)，然后再把坐标看成 2位2进制
数，依次将这 4个点编号为 0，1，3，2即可。 
对于 3维空间，同样我们可以将立方体的一个顶点与原点重合，并使得所有
棱均平行于坐标轴，然后分别确定这8个点的坐标，最后把3维空间内的坐标看
成一个3位2进制数即可。对于D维空间，以此类推。 
现在对于一个 N 个点M条边的无向图（每个点从 0到N-1编号），Will 希望
知道这个图是否同构于一个超立方图。
## 输入格式
第一行包含一个整数 Q表示此数据中一共包含 Q个询问。
接下来 Q组询问，每一组询问的输入格式如下：
第一行包含两个整数 N 和M，
接下来 M 行，每行 2 个不同的整数 x，y，表示图中存在一条无向边连接编
号为x和y的点（0 < = x,y < N）
Q<=3,N<=32768,M<=1000000
## 输出格式
对于每一个询问分别输出一行，内容如下： 
1、如果询问中给定的图不同构于任何一个超立方图，输出-1； 
2、如果同构于某一个超立方图，那么请给图中这N 个点重新编号，并在这
一行输出 N 个用空格隔开的整数，表示原图中每个点新的编号，使得重新编号
后，满足题目中所述的结论。 
注意：输出文件的每一行，要么仅包含一个整数-1，要么则应包含一个由 0
到N-1这 N 个数组成的排列。如果有多组解输出任意一个均可。

```input13
2 2
0 1
1 0
4 4
0 1
1 2
2 0
0 3
8 12
2 3
2 6
7 6
1 7
4 1
3 4
0 2
7 3
5 6
5 1
5 0
4 0

```

```output1-1
-1
0 6 1 5 4 2 3 7
【样例说明】
超立方图中显然是不能有重边的，所以第一个样例是无解的。
```

## 提示
没有写明提示
## 题目来源
By 佚名上传 鸣谢ScarletMoon提供SPJ

