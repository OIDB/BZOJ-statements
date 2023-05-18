## 题目描述

有 $n$ 个可爱的小猴子，有一天，妈妈摘了 $m$ 个桃子，可是怎么分都分不平均。于是妈妈偷偷地把桃子藏了起来，准备第二天再想办法。

可是孩子们到了晚上，纷纷去偷吃。第一只猴子去的时候发现把桃子分成 $n$ 份相等的量，会剩下 $1$ 个桃子，于是拿走了自己的一份，并把多余的 $1$ 个桃子也拿走了。第二只猴子去的时候发现平分成 $n$ 份时会剩下 $2$ 个桃子，于是拿走了自己的一份，并把多余的 $2$ 个桃子也拿走了……第 $k$ 只猴子去的时候发现平分成 $n$ 份时会剩下 $k$ 个桃子，于是拿走了自己的一份，并把多余的 $k$ 个桃子也拿走了，第 $k+1$ 只猴子去的时候发现平分成 $n$ 份后只剩下 $1$ 个桃子，于是拿走了自己的一份，并拿走了多余的 $1$ 个桃子，第 $k+2$ 只猴子去的时候发现平分成 $n$ 份后剩下 $2$ 个桃子，于是拿走了自己的一份，并拿走了多余的 $2$ 个桃子……如此 $k$ 个一循环。第 $n$ 个猴子去的时候，把剩下的桃子（至少一个）全都吃了。

试问 $m$ 至少是多少？ 任务：输入正整数 $n,k(k<n)$，求出最小的正整数 $m$，桃子不能分割。

## 输入格式

输入仅包含一行，包括两个用空格隔开的正整数 $n,k$。

## 输出格式

输出一个正整数，表示最小的 $m$，答案有可能超过 $2^{64}$。

## 样例输入

```plain
4 3
```

## 样例输出

```plain
73
```

## 数据规模与约定

$30\%$ 的数据满足：$0<k<n<12$。

另外 $15\%$ 的数据满足：$k+1=n$。

$100\%$ 的数据满足：$0<k<n<100$。