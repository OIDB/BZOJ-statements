
<h2>

    题目描述
</h2>

<p>

    给定一个无线网络。每一个无线网络的节点都有一个发射半径 $r_{i}$，只要两个节点的Euclid距离 $\leq$ 发射节点的半径，另外一个节点就能接收到信息。
</p>

<p>

    现在所有的节点都使用制度$A$进行信息传输，但现在有一个新的，更好的制度 $B$ 可用，我们考虑将某些节点更新为使用制度 $B$。
    这里有一个限制，如果节点 $T$ 使用制度 $B$，那么所有可以接收到节点 $T$ 信息的节点都必须使用制度 $B$，反之则不一定。
</p>

<p>

    你的任务是选择一些节点进行更新。因为更新节点需要一定的费用，并且可以获得一定的收益，我们用 $score_{i}$ 来衡量节点 $i$ 的收益。我们希望所有更新的节点的 $score$ 之和最大。
</p>


<h2>

    输入格式
</h2>

<p>

    第一行，数据组数T。每组数据以一个整数 $N$ 开始，接下来 $N$ 行每行 $4$ 个整数：$x,y,r,s$。他们代表一个节点的坐标 $(x,y)$，发射半径 $r$ 和 $score - s$ 。
</p>

<h2>

    输出格式
</h2>

<p>

    对于每组数据，输出：Case  #X:score，其中X表示数据编号，从1开始，score表示该组数据的答案。
</p>


<h2>

    提示说明
</h2>

<p>

    $1\le T\le 55,-10000\le x,y\le10000,1\le r\le20000,-1000\le s\le1000,1\le n\le500$
</p>


```input1
1
5
0  1  7  10
0  -1  7  10
5  0  1  -15
10  0  6  10
15  1  2  -20

```
```output1
Case  #1:5
```
