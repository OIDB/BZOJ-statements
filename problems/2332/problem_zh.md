


## 题目描述
坚果保龄球是植物大战僵尸中的一个小游戏。现在疯狂戴夫只给了 **lxhgww**  **一些最普通的坚果，让**  **lxhgww**  **像保龄球一样把坚果扔出去，砸死院子里的僵尸。** 
院子一共由 **N**  **条轨道组成，从上到下依次编号从**  **1**  **到**  **N**  **，每条轨道又被分成若干格。院子里一共有**  **M**  **只僵尸，每只僵尸站在某个格子内，并且可以认为它的位置不会变化。游戏可以分成**  **K**  **个回合，在每个回合中，你可以选择一条轨道，把一个坚果扔出去。被扔出去的坚果首先会沿着轨道直线的从左往右滚动，直到撞到第一只僵尸之后，它开始沿着**  **45**  **度的斜线滚动，并且向中心的一侧滚动（即前**  **N/2**  **行的向右下滚动，后**  **N/2**  **行的向右上滚动，题目保证**  **N**  **是偶数）。院子的两边是围墙。斜着走的坚果撞到围墙或者僵尸会反弹，即从往右上走变成往右下走，或者反过来。直到坚果不再能打到任何僵尸之后，该回合结束。注意：多只僵尸可能站在同一格，这个时候坚果每次只会撞死该格子的其中一只僵尸。** 
为了砸死尽量多的僵尸，现在 **lxhgww**  **决定在每回合的开始，选择在当前情况下可以砸死最多僵尸的一条路线扔出坚果。在出现相同的情况时，他会选择编号最小的轨道扔出。为了了解这个做法的效果，现在**  **lxhgww**  **需要你帮助他计算这个方法可以砸死的僵尸数目。** 
## 输入格式
输入的第一行有 **3**  **个整数，**  **N**  **，**  **M**  **，**  **K**  **。** 
接下来 **M**  **行，每行两个整数**  **X** i, Yi，表示第 **i**  **个僵尸位于第**  **Y** i条轨道，从左数第 **X** i个格子中。
## 输出格式
 
输出数据包括 **K+1**  **行。** 
前 **K**  **行，每行**  **2**  **个数据**  **A** i, Bi，表示在第 **i**  **个回合，从第**  **A** i条轨道扔出坚果，这个坚果在运行过程中打到了 **B** i个僵尸。
最后一行是一个数字，表示被打到的僵尸总数。

```input1
4 2 1
1 2
5 2

```
```output1

2 2

2
```

## 提示
【数据范围】
对于20%的数据，保证： N<=200，M<=500，K<=200，Xi<=200；
对于50%的数据，保证： N<=200，M<=200000，K<=200，Xi<=1000000；
对于100%的数据，保证： N<=20000，M<=200000，K<=100000，Xi<=1000000；
对于所有的数据，保证：1<=Yi<=N
## 题目来源
Day1

