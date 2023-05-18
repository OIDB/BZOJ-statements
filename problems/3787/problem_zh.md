## 题目描述

Autumn 终于会求区间逆序对了！Bakser 神犇决定再考验一下他，他说道：“在 Gty 的妹子序列里，某个妹子的美丽度可也是会变化的呢。你还能求出某个区间中妹子们美丽度的逆序对数吗？当然，为了方便，这次我们规定妹子们的美丽度在 $[1,n]$ 中。仍然强制在线。”

Autumn 需要你的帮助。

给定一个正整数序列 $a_1 \dots a_n$，支持单点修改，对于每次询问，输出 $a_l \dots a_r$ 中的逆序对数，强制在线。

## 输入格式

第一行包括一个整数 $n$，表示数列 $a$ 中的元素数。

第二行包括 $n$ 个整数 $a_1 \dots a_n$。

接下来一行包括一个整数 $m$，表示操作的个数。

接下来 $m$ 行，每行包括 $3$ 个整数。

`0 L R` 询问 $[L,R]$ 中的逆序对数。

`1 p v` 将 $p$ 位置的数修改为 $v$。

$L,R,p,v$ 都需要异或上一次的答案，保证异或之后的值是合法的。

保证涉及的所有数在 `int` 内。

## 输出格式

对每个询问，单独输出一行，表示 $a_l \dots a_r$ 中的逆序对数。对每个询问，单独输出一行，表示 $a_l \dots a_r$ 中的逆序对数。

```input1
10
1 7 5 6 9 4 9 4 4 7
10
0 4 6
0 5 8
0 1 10
1 25 19
0 19 25
1 14 4
0 12 12
0 2 5
1 8 7
1 1 10
```

```output1
2
3
16
13
0
2
```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 5 \times 10^4$，$1 \le m \le 5 \times 10^4$，$1 \le a_i \le n$，$1 \le L \le R \le n$，$1 \le p \le n$，$1 \le v \le n$。

## 题目来源

By Autumn
