## 题目描述

在约翰的农场上每个新出生的奶牛都有一个 $N$ 位的数字，这些数字是连续的，这个数字大于任何其他的奶牛，也就是说，数字越大这头牛也就越年轻。

每头奶牛都对自己的编号非常感兴趣。奶牛因自己编号中一半以上（一半除外）数字相同而感到自豪。比如 $23522$ 中，数字 $2$ 在 $5$ 个数字中出现了 $3$ 次，而 $12342$ 中没有一个数字出现超过半数。那些一半以上数字相同的数叫特殊数，其他的叫普通数。当然，普通的奶牛非常嫉妒特殊的奶牛，过去它们经常欺负特殊奶牛。由于身体的缘故，一头奶牛只能欺负比他小的奶牛。事实上，一头普通奶牛只欺负比他小的特殊奶牛中最大的那头。不幸的是，普通奶牛并不清楚那头应该被他欺负的奶牛到底是谁。给出一头奶牛的编号，确定哪头奶牛应该被他欺负，如果这头奶牛本身是特殊的，输出这头奶牛自己的编号。

## 输入格式

仅一个数，要欺负人的奶牛编号。

## 输出格式

仅一个数，应该被欺负的奶牛编号。

```input1
1234

```

```output1
1311
```

$1$ 在 $1311$ 中出现 $3$ 次，超过半数。$1199$ 不是特殊数，因为 $1$ 和 $9$ 均未超过半数。

## 提示

对于 $100\%$ 的数据，$1 ≤ N ≤ 100$。

## 题目来源

Orange


