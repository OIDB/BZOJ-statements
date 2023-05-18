


## 题目描述
【故事背景】
JSOI王国的地铁又涨价了！正在JSOI旅游的JYY非常不开心L。这次票价
改革后，乘客并不是按照乘坐的距离收费，而是按照换乘次数进行收费的！JYY
也要按此更新他的线路搜索软件了。
JYY心想，在支付同样票价的前提下，岂不是坐的站数越多，自己就赚的越
多嘛！于是JYY希望开发一个线路搜索软件，使得自己总能够“赚”的最多！
JSOI地铁一共有N条线路S个车站。第i条地铁线路包含Li个站。所有地铁
线路都是一条从首发站到终点站的直线型线路（不存在例如北京地铁2号线或者
10号线那样奇葩的环线）。同时，每一条地铁线路都是双向运行的。
如果有不同的线路经过同一个地铁站，那么乘客就可以在那个地铁站进行换
乘。根据JSOI地铁的最新收费方式，每当乘客进入一列正在运行的地铁列车，
都需要支付1的费用。
因此，假设乘客一共换乘了x次，那么就需要总共支付x+1的乘车费用。
由于地铁线路都是双向运行的，因此在任意一站都可以换乘该线地铁反方向
运行的列车。不过，需要注意的是，即使是换乘同样线路的反方向列车，也是需
要付费的（因为总是需要先下车，再重新上车的）。
JYY现在要从A站坐地铁前往B站。假设对于任意一条地铁线路，相邻两
站间地铁的运行时间均为1分钟，并且列车停站和换乘均不耗时间，JYY想知道
1)他最少需要支付的票价是多少钱；
2)在支付最少票价的前提下，他最多可以乘坐多少分钟的地铁。
## 输入格式
第一行包含两个正整数N和S；
第二行包含S个由空格隔开的字符串，表示S个站点的站名；每个字符串长
度不超过40，并且仅包含字母，数字，以及横线‘-’；
接下来N行，每行描述一条地铁线路；
对于其中第i行，首先包含一个正整数Li，接下来Li个字符串，表示这条地
铁线路上的站点名称；一条线路允许多次停靠同一个站点。
第N+3行，包含两个不同的字符串A和B，表示JYY目前在A站，希望坐
地铁前往B站。
2<=N<=50,000,S<=3∗10N,Sigma(iLi)<=8∗10^5。
输入数据保证，所有站名的长度总和不超过7∗10^5
## 输出格式
第一行包含一个整数C，表示JYY最少需要支付的乘车费用；
第二行包含一个整数T，表示JYY在花费C的前提下，可以乘坐地铁的最长时间。
如果不存在两个站点之间的路线，第一行输出“-1”，第二行输出“0”（均不包含引号）。

```input1
2 5 
A B C D E 
4 A B C D 
3 C D E 
A D 

```

```output1
1
3
```

## 提示
没有写明提示
## 题目来源
没有写明来源

