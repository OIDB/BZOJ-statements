


## 题目描述
Farmer John needs your help deciding where to build a fence in the shape of a straight line to help 
restrict the movement of his cows. He has considered several possible fence locations and needs your 
help to determine which of these are usable, where a fence is considered usable if all of the cows 
are on the same side of the fence. A fence is not usable if there is a cow that lies directly on it. 
FJ will be asking you a number of queries regarding possible fence locations; a query should be 
answered "YES" if it corresponds to a usable fence location, "NO" otherwise.
Additionally, FJ may occasionally bring new cows into the herd. When a new cow joins the herd, all 
fence queries from that point onward will require her to be on the same side of a fence as the rest 
of the herd for the fence to be usable.FJ需要你帮助他决定在哪里建造形状是一条无限长的直线的栅栏来限制
他的牛的活动。他选出了几个可能的建造栅栏的位置，你需要帮助他判断哪些栅栏是有用的。一个栅栏是有用的当且
仅当所有奶牛都在栅栏的同一侧(如果有牛群在栅栏所在的直线上，那么栅栏是没用的)，FJ将会问你一些问题，如果
这个栅栏是有用的，需要输出“YES”，反之输出“NO”。 另外，FJ也可能会带来一些新的奶牛加入这个牛群。一头牛
加入之后，以后的所有询问中，这头牛也需要与其它的牛在栅栏的同一侧。 
## 输入格式
The first line of input contains N (1 <= N <= 100,000) and Q (1 <= Q <= 100,000) separated by a space. 
These give the number of cows initially in the herd and the number of queries, respectively.
The following N lines describe the initial state of the herd. Each line will contain two space separated 
integers x and y giving the position of a cow.
The remaining Q lines contain queries either adding a new cow to the herd or testing a fence for usability. 
A line of the form "1 x y" means that a new cow has been added to the herd at position (x, y). A line of 
the form "2 A B C" indicates that FJ would like to test a fence described by the line Ax + By = C.
All cow positions will be unique over the whole data set and will satisfy (-10^9 <= x, y <= 10^9). 
Additionally the fence queries will satisfy -10^9 <= A, B <= 10^9 and -10^18 <= C <= 10^18. No fence 
query will have A = B = 0.
第一行包含两个用空格隔开的整数N和Q代表最开始奶牛的数目和FJ的提问的个数。 
接下来的N行每行包含两个整数x和y，代表每只奶牛的坐标 
最后的Q行，每行代表一个提问，形如“1 x y”的提问代表FJ在坐标为(x,y)的位置放置了一头新的奶牛。形如"2 A B C"的
提问代表FJ向你询问位于直线Ax+By+C上的栅栏是否是有用的。
## 输出格式
<h4>

For each fence query, output "YES" if the fence is usable. Otherwise output "NO".
**对于每个形如“2 A B C”的提问，输出一行。 ** 
**如果栅栏是有用的，输出"YES"，否则输出"NO"(不包含引号)。** 
</h4>


```input13 4
0 0
0 1
1 0
2 2 2 3
1 1 1
2 2 2 3
2 0 1 1

```

```output1YES
NO
NO
```

## 提示
 数据范围： 
1<=N<=100000 , 1<=Q<=100000 
-109<=x,y<=109 
-109<=A,B<=109 
-1018<=C<=1018 
输入数据保证所有奶牛的坐标都是互不相同的，而且不会出现A=B=0的询问。 
样例解释: 
最开始的三头牛都在2x+2y=3这条直线同侧，但是奶牛(1,1)加入后，与其它三头牛不在同一侧，所有第二个栅栏是没用的。因为奶牛(0,1)和奶牛(1,1)在直线y=1上，所以第三个栅栏是没用的 
## 题目来源
Gold


