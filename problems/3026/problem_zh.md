## 题目描述

现在要建造一些 $ n $ 层的楼梯，它从上往下依次有 $ 1,2,3...n $ 个块组成。也就是说一个 $ n $ 层的楼梯有 $ \displaystyle \frac {n(n+1)}{2} $ 块。

现在有许多各种各样的整块可以用来建造楼梯。现规定一个 $ n $ 层的楼梯只能用N个整块来，如下三层的，有五种方法。现在我们有 $ k $ 种染料，要对这所有的楼梯进行涂色。

每种方案可以任意选择一种染料来涂色，所有的颜色不一定全要用上。

你需要计算出涂色的总方案数。请输出答案  $ \mod 1000000123 $。

## 输入格式

输入有多组数据，做到文件底结束。
每个数据一行，为 $ n,k $。

## 输出格式

如题

## 样例输入

```
3 2
2 2
1 1
```

## 样例输出

```
32
4
1
```

## 提示

对于 $ n=3,k=2 $ 这组数据，一共有 $ 5$ 种建造方案，那么答案就是 $ 2^5=32 $。

## 数据规模与约定

对于 $100\%$ 的数据，$ 1\leq n \leq 1\times 10^9 $，$ 1\leq k \leq 1\times 10^9 $。

