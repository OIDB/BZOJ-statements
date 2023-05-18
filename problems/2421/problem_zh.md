## 题目描述

话说今年 HNOI 省队集训在一中进行，为此 fmsoi 特意准备了一个巨大的电子广告牌，准备在上面写“一中欢迎你”。但是这块牌子却出现了问题，经过神一般的小 Y 的修理后，终于好了，可是却恢复到了默认状态——没有显示任何字了，显然我们还要让它显示出“一中欢迎你”。

众所周知，这类广告牌通常由若干像素点构成，我们考虑其中的一行，最开始每一行都是不发光的。

每一行有 $N$ 个像素点，将其标号 $1 ... N$ 。现在给定 $K$ 个点，要求这 $K$ 个点发光，其余点不能发光。而这个电子广告牌的操作方式比较畸形，它有 $L$ 种操作方法，第 $i$ 种为 $U_{i}$ ，即你能将任意长为 $U­­_{i}$ 的连续一段的像素状态取反，即改变发光状态。

现在你被分配了要处理好不同的 $T$ 行，为了节省时间，对于每一行你都必须用最少的操作次数。

## 输入格式

**本题有多组测试数据。**

第一行一个数 $T$ ，表示数据组数。

然后是 $T$ 组数据描述，对于每组数据：

第一行为 $N,K,L$ ，即一行有 $N$ 个点，要求 $K$ 个点必须发光，有 $L$ 种操作方式。

第二行 $K$ 个数，表示要求发光的 $K$ 个点。

第三行 $L$ 个数，表示 $L$ 种操作。

## 输出格式

包含 $T$ 个数，每个一行，即对于每一组数据的最少操作次数。

如果无法完成，请输出 ``-1`` 。

```input1
2
10 8 2
1 2 3 5 6 7 8 9
3 5
3 2 1
1 2
3
```

```output1
2
-1
```

## 数据规模与约定

有 $20 \%$ 较小的数据。

对于$100 \%$ 的数据，保证 $1\le T\le 10 , 1\le N \le 10^4 , 1\le K \le 10 , 1\le L \le 100 , 1\le U_i \le N$ 。