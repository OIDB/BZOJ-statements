## 题目描述

一个 $ n $ 位数是handsome的，当且仅当其中只有 $ 0,1,2 $，而且相邻的两个数构成的数对不在危险集合中。

$ n $ 位数 $ A $ 在排列 $ P $ 的意义下字典序小于 $ B $，如果存在一个 $ k $ 使得 $ A[P[1]]=B[P[1]],A[P[2]]=B[P[2]]..A[P[k]]=B[P[k]],A[P[k+1]]<B[P[k+1]] $。

给定 $ n $，危险集合，一个排列 $ P $ ，以及一个handsome数 $ T $，统计在排列 $ P $ 意义下小于 $ T $ 的handsome数的个数。输出答案模 $ 10^9+7 $ 的值。

## 输入格式

输入的第一行为 $ n $。

接下来一行 $ n $ 个整数，表示排列 $ P $。

接下来一行一个整数 $ m $ ，表示危险集合中数对的个数。接下来一行 $ m $ 对数，表示危险集合

最后一行为 $ T $。

## 输出格式

一个整数，表示在排列 $ P $ 意义下小于 $ T $ 的handsome数的个数。

## 样例输入

```
3
2 1 3
2
22 13
321
```

## 样例输出

```
9
```

## 数据规模与约定

对于 $100\%$ 的数据， $ n\leq 4\times 10^5 $ ， $ m\geq 1 $ ，保证 $ T $ 是handsome数。

## 题目来源

Dragonite提供翻译

