## 题目描述

在舞台上有 $n$ 个枪手，第 $i$ 个枪手瞄准了第 $p_i$ 个枪手，将于第 $u_i$ 秒开枪。一个枪手如果成功开枪， 那么被瞄准的枪手会立刻死亡。

现在给出 $q$ 次对于 $u$ 的单点修改操作，请在一开始和每次修改操作后统计出最后存活的枪手个数。

## 输入格式

第一行一个正整数 $n$，表示枪手的个数。 

第二行包含 $n$ 个互不相同的正整数 $p_{1\cdots n}$，依次表示每个枪手的目标。

第三行包含 $n$ 个正整数 $u_{1\cdots n}$，依次表示每个枪手的开枪时间。

接下来一行包含一个正整数 $q$，表示修改操作的个数。

接下来 $q$ 行，每行包含两个正整数 $k,v$，表示把 $u_k$ 修改为 $v$。

数据保证任何时刻任意两个枪手的开枪时间都不同。

## 输出格式

第一行包含一个正整数，即在进行修改之前最后存活的枪手个数。

接下来 $q$ 行，每行包含一个正整数，第 $i+1$ 行输出在第 $i$ 次修改之后最后存活的枪手个数。

```input1
4
2 3 4 1
1 2 3 4
3
1 8
2 7
3 6
```

```output1
2
2
1
1
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n\leq 2\times 10^5$，$1\leq p_i,k\leq n$，$p_i\not =i$，$1\leq u_i,v\leq 10^9$。

数据保证任何时刻任意两个枪手的开枪时间都不同。