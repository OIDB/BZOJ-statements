## 题目描述

打孔机是一种在票上打孔的装置， 假设票是一个 $M \times N$ 的矩阵，矩阵行列间距相等，你可以选择在 $M \times N$ 个位置上打穿或不打穿，这样就有 $2^{M \times N}-1$（至少要打一个孔）不同的方案数。

但是我们的问题并不是这么简单的，如果两种方案经过如下的若干操作后，打穿的孔刚好重合，那么认为这两个方案是相同的：

-   翻转；
-   旋转 $0 \degree ,90 \degree,180 \degree,270\degree$；
-   平行移动；

显然如果两种方案上孔的数目不同，那么必然是不同的方案。现在你的问题就是给定 $M,N$，算出所有不同的方案数。

## 输入格式

文件包含两个数 $M~(M \leq 6),~N~(N \leq 10)$ ,用空格分开。

## 输出格式

只有一行，为所求的方案数。

```input1
3 3
```

```output1
85
```