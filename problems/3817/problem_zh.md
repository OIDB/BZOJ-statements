## 题目描述

给定整数 $n,r$，求 $\sum_{d=1}^n(-1)^{\lfloor\sqrt{d\times r\times d}\rfloor}$。

## 输入格式

第一行一个整数 $T$ 表示数据组数。

接下来 $T$ 行，每行两个整数 $n,r$ 表示一组数据。

## 输出格式

共 $T$ 行，第 $i$ 行一个整数表示第 $i$ 组数据的答案。

```input1
3
3 5
3 6
3 7
```

```output1
3
1
-1
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n\leq 10^9$，$1\leq r\leq 10^4$，$1\leq T\leq 10^4$。

## 来源

$2015$ 年国家集训队测试。
