## 题目描述

贝茜和其他奶牛联系是通过一连串的中间奶牛传递的，所以当第一头牛和贝茜联系，第二头牛和第一头牛联系，第三头牛和第二头牛联系，以此类推，贝茜就能依次联系到其中的每一头奶牛。联系长度是指传递过程中涉及的奶牛的数目（不包括贝茜）。任何一头奶牛（不包括贝茜）的培根距离是指从贝茜到该奶牛的最小联系长度。最小的培根距离是 $1$（当贝茜能够直接与该奶牛联系时）。约输有 $C$ 头牛，编号 $1$ 到 $C$ ，贝茜是 $1$ 号。有$P$ 组奶牛相互联系．请找到最大的培根距离．

## 输入格式

第 $1$ 行：$C$ 和 $P$ 。

第 $2$ 到 $P+1$ 行：每行两头牛，它们之间有联系。

## 输出格式

输出最大培根距离．

```input1
1 2
2 3
2 4
3 4
3 5
4 5
6 5
```

```output1
4
```

## 提示

从贝茜到 $6$ 号奶牛的距离是 $4$ ，联系路径 $(2,4,5, 6)$ 和 $(2,3,5,6)$ 都适合

## 数据范围与约定

对于 $100\%$ 的数据， $1 \leq P \leq 10000$。

