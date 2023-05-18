## 题目描述

初始时滑冰俱乐部有 $1$ 到 $n$ 号的溜冰鞋各 $k$ 双。已知 $x$ 号脚的人可以穿 $x$ 到 $x+d$ 的溜冰鞋。 有 $m$ 次操作，每次包含两
个数 $r_i,x_i$ 代表来了 $x_i$ 个 $r_i$ 号脚的人。$x_i$ 为负，则代表走了这么多人。 对于每次操作，输出溜冰鞋是否足够。

## 输入格式

第一行四个整数 $n,m,k,d$。

接下来 $m$ 行，每行两个数 $r_i,x_i$。

## 输出格式

对于每个操作，输出一行，`TAK` 表示够，`NIE` 表示不够。

```input1
4 4 2 1
1 3
2 3
3 3
2 -1
```

```output1
TAK
TAK
NIE
TAK
```

## 数据规模与约定

$ 1 \le n \le 2 \times 10^5 , 1 \le m \le 5 \times 10^5 , 1 \le k \le 10^9, 0 \le d \le n$

$1 \le i \le m, 1 \le r_i \le n-d , |x_i| \le 10^9$