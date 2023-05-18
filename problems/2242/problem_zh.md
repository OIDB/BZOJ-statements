<h2>题目描述</h2>

你被要求设计一个计算器完成以下三项任务：

1. 给定 $y,z,p$，计算 $y^z \bmod p$ 的值；
2. 给定 $y,z,p$，计算满足 $xy \equiv z \pmod p$ 的最小非负整数 $x$；
3. 给定 $y,z,p$，计算满足 $y^x \equiv z \pmod p$ 的最小非负整数 $x$。

为了拿到奖品，全力以赴吧！

<h2>输入输出格式</h2>

<h3>输入格式</h3>


输入文件包含多组数据。

第一行包含两个正整数 $T,K$，分别表示数据组数和询问类型（对于一个测试点内的所有数据，询问类型相同）。

以下 $T$ 行每行包含三个正整数 $y,z,p$，描述一个询问。

<h3>输出格式</h3>


输出文件包括 $T$ 行。

对于每个询问，输出一行答案。

对于询问类型 2 和 3，如果不存在满足条件的，则输出 `Orz, I cannot find x!`。

<h2>输入输出样例</h2>


```input1
3 1
2 1 3
2 2 3
2 3 3
```

```output1
2
1
2
```

```input2
3 2
2 1 3
2 2 3
2 3 3
```

```output2
2
1
0
```

```input3
4 3
2 1 3
2 2 3
2 3 3
2 4 3
```

```output3
0
1
Orz, I cannot find x!
0
```


## 说明

测试点共分为三类，各类测试点占总测试点的比例如下：

| $K=$ | 测试点占比 |
| :--: | :--------: |
| $1$  |   $20\%$   |
| $2$  |   $35\%$   |
| $3$  |   $45\%$   |

所有数据均满足：$1 \leq y,z,p \leq 10^9$，$p$ 是质数，$1 \leq T \leq 10$。