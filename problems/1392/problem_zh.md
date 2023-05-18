## 题目描述

给出一个 $n\times m$ 的矩形。

在它上面有两种辐射点，`black` 及 `white`，每个点都有自己的辐射范围。

对于其它的点，如果它受到白点的辐射多于黑色的，则为白点，反之亦然，如果相同的话则中立。

现给出白点及黑色的坐标及各自的辐射范围，问最后白色点一共有多少个，黑色点共有多少个。

## 输入格式

第一行给出 $n$ 和 $m$，左下角坐标为 $(0,0)$，右上角为 $(n-1,m-1)$。

第二行给出数字 $k$ ，代表有多少个辐射点。

接下来 $k$ 行，每行先给出辐射点的属性，用一个字符 `W` 或 `B` 表示；再给出坐标 $(x_i,y_i)$，再给出辐射范围 $p_i$。

## 输出格式

两个数，分别代表白色点有多少个，黑色点有多少个。


```input1
10 10
3
W 3 6 3
B 6 4 2
W 3 3 2
```


```output1
30 9
```

## 样例说明 

![](file://pic1.jpg)



## 数据规模与约定

对于 $100\%$ 的数据，$1 \leq n,m \leq 10^9$，$0 \le k \leq 3\times 10^3$，$0 \leq x_i< n$，$0\leq y_i< m$，$p_i\in[0, 5\times 10^8)$。
