## 题目背景

在美丽富饶的 Katharon 国中生活着一群快乐的小木偶。他们衣食无忧，自给自足。然而在某一天，来自外星的 X 国要对 Katharon 国发起攻击，国家安危迫在眉睫，下面请你来做战前的防御准备工作。

## 题目描述

我们定义战线为一条长度为 $n$ 的序列，在这条战线上共设有 $n$ 个检查点，从左到右依次标号 $1$ 到 $n$ 。一个战线为合法战线当且仅当任意一个检查点可以通过安全检查。对于第 $i$ 个检查点可以通过安全检查的方式有两种，第一种是放置一个守卫塔，这将花费 $a_i$ 的费用。第二种方式是放置一个木偶，放置木偶的花费等于这个检查点右侧的第一个守卫塔到它的距离。举例来说，若检查点 $i$ 放置一个木偶，检查点 $i$ 右侧的第一个守卫塔位置为 $j(i<j)$ ，则在点 $i$ 放置木偶的花费为 $j-i$ 。当然，第 $n$ 个检查点只能放置守卫塔，因为它的右面不可能再存在别的守卫塔了。我们定义战线花费为所有守卫塔的花费加上所有木偶的花费，现在 Katharon 国的国王 hzc 君将提供给你每个位置放置守卫塔的费用以及战线的总长度，请你求出最小的战线花费值。

## 输入格式

第一行为一个整数 $n$ 表示战线的总长度。

第二行 $n$ 个整数，第 $i$ 个整数表示在位置i放置守卫塔的花费 $a_i$。

## 输出格式

共一个整数，表示最小的战线花费值。

## 样例输入

```plain
10
2 3 1 5 4 5 6 3 1 2
```

## 样例输出

```plain
18
```

## 数据规模与约定

$1\le n \le10^6,1\le a_i\le 10^9$

## 题目来源

Katharon+#1
