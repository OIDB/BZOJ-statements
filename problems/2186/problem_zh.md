## 题目描述

大富翁国因为通货膨胀，以及假钞泛滥，政府决定推出一项新的政策：现有钞票编号范围为 $1$ 到 $n!$，但是，政府只发行编号与 $m!$ 互质的钞票。房地产第一大户沙拉公主决定预测一下大富翁国现在所有真钞票的数量。现在，请你帮助沙拉公主解决这个问题，由于可能张数非常大，你只需计算出对 $R$ 取模后的答案即可。$R$ 是一个质数。

## 输入格式

第一行为两个整数 $T,R$。

接下来有 $T$ 组数据，对于每一组数据：

第一行两个整数 $n,m$。

## 输出格式

共 $T$ 行，对于每一对 $n,m$，输出 $1$ 至 $n!$ 中与 $m!$ 互质的数的数量对 $R$ 取模后的值。

## 样例输入

```plain
1 11
4 2
```

## 样例输出

```plain
1
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq m\leq n\leq 10^7$，$R\leq 10^9+7$，$1\leq T\leq 10^4$。
