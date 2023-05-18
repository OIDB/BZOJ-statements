## 题目描述

维护一个向量集合，在线支持以下操作：

1.  ``A x y`` ：加入向量 $(x, y)$；
2. ``Q x y l r``：询问第 $L$ 个到第 $R$ 个加入的向量与向量 $(x, y)$ 的点积的最大值。集合初始时为空。

注：向量 $(x, y)$ 和 $(z, w)$ 的点积定义为 $xz+yw$。

## 输入格式
输入的第一行包含整数 $N$ 
和字符 $s$，分别表示操作数和数据类别；  
接下来 $N$ 行，每行一个操作，格式如上所述。

请注意 $s \neq$ `E` 时，输入中的所有整数都经过了加密。你可以使用以下程序得到原始输入：

```cpp
inline int decode (int x long long lastans) {
     return x ^ (lastans & Ox7fffffff);
}
function decode
begin
```

其中 `x` 为程序读入的数，`lastans` 为之前最后一次询问的答案。在第一次询问之前，`lastans`$=0$。

## 输出格式

对每个 $Q$ 操作，输出一个整数表示答案。

```input1
6 A
A 3 2
Q 1 5 1 1
A 15 14
A 12 9
Q 12 8 12 15
Q 21 18 19 18
```
```output1
13
17
17
```

解密之后的输入为
```plain
6 E
A 3 2
Q 1 5 1 1
A 2 3
A 1 4
Q 1 5 1 2
Q 4 3 2 3
```

## 提示

对于所有的数据，$1 \leq N \leq 4 \times 10^5$，操作中的向量坐标满足 $|x|,|y| \leq 10^8$，询问满足 $1 \leq L \leq R \leq T$，其中 $T$ 为已经加入的向量个数。