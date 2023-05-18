## 题目描述

有一枚硬币，抛出正面 `H` 的概率为 $\frac{a}{b}$，抛出反面 `T` 的概率为 $1-\frac{a}{b}$。现在 TT 小朋友开始玩丢硬币的游戏，并且把每次抛出的结果记录下来，正面记为 `H`，反面记为 `T`，于是她得到了一个抛硬币序列 `HTHHT…`。她突然想到一个问题：在抛出正面和反面概率都是 $\frac{1}{2}$ 的情况下，要使得抛出的序列出现目标序列 `HT`，期望要抛多少次。然而经过 $1$ 秒的思考以后她发现，若第一次抛出的是 `T`，那么还需要期望抛出 `HT` 的次数，如果第一次抛出的是 `H`，则期望只需要抛出 `T` 的次数，而期望抛出 `T` 的次数显然是 $2$。她设抛出 `HT` 的期望次数是 $x$，则得到了方程：$x = 1 + (\frac{1}{2} \times x + \frac{1}{2} \times 2)$。

解得 $x = 4$，所以抛出 `HT` 的期望次数是 $4$ 次。

她在解决了这个弱化很多的问题以后，开始思考对于一般情况下，抛出正反面的概率不一定相同，且抛出的目标序列不一定为 `HT` 时需要的期望步数。然而经过很长一段时间的苦思冥想仍然无果，于是她开始求助于你。

## 输入格式

第一行两个数 $a,b$。意义如题目描述。

接下来一行一个只包含 `H` 和 `T` 的字符串 $s$。表示要抛出的目标序列。

## 输出格式

输出仅一行 `p/q` ，其中 $p$ 和 $q$ 均为正整数且互质，表示抛出目标序列 $s$ 所需要的期望步数。

注意，若 $q$ 为 $1$ 时，不省略 `/1`。

```input1
1 2
HT
```

```output1
4/1
```

## 数据规模与约定

* $100\%$ 数据 $1 \leq a < b < 100$，$|s| \leq 1000$。