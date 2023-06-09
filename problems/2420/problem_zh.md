## 题目描述

堆积木是小 Y 很喜欢的一款游戏。有 $N$ 种颜色（颜色标号为 $1$ 到 $N$ ）的积木，我们规定， 在堆放积木**第 $I$ 列只能放第 $I$ 种颜色**的积木，如图 $1$（白色为空）。

![](https://hydro.org.cn/d/bzoj/p/2420/file/pic2.png)

小 Y 每次可以选三块颜色都不同的积木，$N$ 种颜色共有 $C(N,3)$ 种选法。对于每次操作，将选出的三块积木堆在已经摆好的积木上。**对于同种颜色的积木，如果之前已经存在了一个积木，那么就将这块积木和选出的积木一起消去**。图 $1$ 消去后就变成图 $2$ 。

![](https://hydro.org.cn/d/bzoj/p/2420/file/pic3.png)

游戏开始前有一些积木，为了简化游戏，规定每种颜色的积木初始数量不超过 $1$ 。小 Y 操作 $M$ 次后，如果剩下的状态和小 X 给的状态一样，那么小 Y 就赢了。但小 Y 觉得赢了还不够过瘾，他想知道有多少种方法可以获胜。

如果 $A$ 方案的某次操作在 $B$ 方案中没有出现，那么 $A,B$ 方案可视为不同。由于答案会很大，请对 $10007$ 取模。

## 输入格式

第一行有两个数 $N,M$ ，表示有 $N$ 种颜色，$M$ 次操作。

第二行有 $N$ 个数，$0$ 和 $1$ ，表示初始状态。

第三行有 $N$ 个数，$0$ 和 $1$ ，表示最终状态。

注意 $1$ 表示有，$0$ 表示无。

## 输出格式

仅包含一个数，表示方案数，如果不能获胜，输出 $0$ 。

```input1
4 3
1101
1001
```

```output1
1
```

## 提示

一种方案中不能重复选同一组积木，比如之前选过了 $(1,2,3)$ 就不能再选了，$(1,3,4)$ 和 $(1,2,4)$ 是可以选的。

## 数据规模与约定

对于 $100 \%$ 的数据，保证 $1 \le N \le 1000 , 0 \le M \le 1000$ 。
