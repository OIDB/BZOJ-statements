

## 题目描述
给定一个长度为 $n$ 且值全部为 $0$ 的序列，下标从 $0$ 开始。有两种类型操作：

- `1 l r h`：将序列 $[l,r]$ 中的所有小于 $h$ 的元素修改为 $h$。

- `2 l r h`：将序列 $[l,r]$ 中所有大于 $h$ 的元素修改为 $h$。
## 输入格式
第一行两个整数 $n,k$，分别表示序列长度和操作次数。

接下来 $k$ 行，每行表示一个操作。
## 输出格式
一行 $n$ 个整数，表示经过 $k$ 次操作后最终的序列。
```input1
10 3
1 3 4 91220
1 5 9 48623
2 3 5 39412
```

```output1
0
0
0
39412
39412
39412
48623
48623
48623
48623
```
```input2
10 6
1 1 8 4
2 4 9 1
2 3 6 5
1 0 5 3
1 2 2 5
2 6 7 0
```

```output2
3
4
5
4
3
3
0
0
1
0
```

## 提示
对于 $100\%$ 的数据，$1\le n\le 2\times 10^6$，$1\le k\le 5\times 10^5$，$1\le h_i\le 10^5$。