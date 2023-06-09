## 题目描述

为了随时与 rainbow 快速交流，Freda 制造了两部传呼机。Freda 和 rainbow 所在的地方有 $ n $ 座房屋、$ m $ 条双向光缆。每条光缆连接两座房屋，传呼机发出的信号只能沿着光缆传递，并且传呼机的信号从光缆的其中一端传递到另一端需要花费 $ t $ 单位时间。现在 Freda 要进行 $ q $ 次试验，每次选取两座房屋，并想知道传呼机的信号在这两座房屋之间传递至少需要多长时间。Freda 和 rainbow 简直弱爆了有木有 T_T，请你帮帮他们吧……

$ n $ 座房屋通过光缆一定是连通的，并且这 $ m $ 条光缆有以下三类连接情况：

* 光缆不形成环，也就是光缆仅有 $ n-1 $ 条。
* 光缆只形成一个环，也就是光缆仅有 $ n $ 条。
* 每条光缆仅在一个环中。

## 输入格式

第一行包含三个用空格隔开的整数，$ n,m $ 和 $ q $。

接下来 $ m $ 行每行三个整数 $ x $、$ y $、$ t $，表示房屋 $ x $ 和 $ y $ 之间有一条传递时间为 $ t $ 的光缆。

最后 $ q $ 行每行两个整数 $ x $、$ y $，表示 Freda 想知道在 $ x $ 和 $ y $ 之间传呼最少需要多长时间。

## 输出格式

输出 $ q $ 行，每行一个整数，表示 Freda 每次试验的结果。

## 样例输入 #1

```
5 4 2
1 2 1
1 3 1
2 4 1
2 5 1
3 5
2 1
```

## 样例输出 #1

```
3
1
```

## 样例输入 #2

```
5 5 2
1 2 1
2 1 1
1 3 1
2 4 1
2 5 1
3 5
2 1
```

## 样例输出 #2

```
3
1
```

## 样例输入 #3

```
9 10 2
1 2 1
1 4 1
3 4 1
2 3 1
3 7 1
7 8 2
7 9 2
1 5 3
1 6 4
5 6 1
1 9
5 7
```

## 样例输出 #3

```
5
6
```

## 数据规模与约定

对于 $100\%$ 的数据，$ 2\leq n\leq 1\times 10^4 $，$ n-1\leq m\leq 1.2\times 10^4 $，$ q=1\times 10^4 $，$ 1\leq x,y\leq n $，$ 1\leq t<32768 $。

## 题目来源

Poetize9

