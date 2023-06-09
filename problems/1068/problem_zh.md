## 题目描述

给一个由小写字母组成的字符串，我们可以用一种简单的方法来压缩其中的重复信息。压缩后的字符串除了小写字母外还可以（但不必）包含大写字母 `R` 与 `M`，其中 `M` 标记重复串的开始，`R` 重复从上一个 `M`（如果当前位置左边没有 `M`，则从串的开始算起）开始的解压结果（称为缓冲串）。例如 `abcabcdabcabcdxyxyz` 可以被压缩为 `abcRdRMxyRz`。

## 输入格式

输入仅一行，包含待压缩字符串，仅包含小写字母，长度为 $n$。

## 输出格式

输出仅一行，即压缩后字符串的最短长度。

```input1
aaaaaaa
```

```output1
5
```

```input2
bcdcdcdcdxcdcdcdcd
```

```output2
12
```

## 提示

在第一个例子中，解为 `aaaRa`，在第二个例子中，解为 `bMcdRRxMcdRR`。

$50\%$ 的数据满足：$1\leq n\leq 20$。

$100\%$ 的数据满足：$1\leq n\leq 50$。

## 题目来源

没有写明来源