## 题目描述

监狱有 $n$ 个房间，每个房间关押一个犯人，有 $m$ 种宗教，每个犯人会信仰其中一种。如果相邻房间的犯人的宗教相同，就可能发生越狱，求有多少种状态可能发生越狱。

答案对 $10^5 + 3$ 取模。

## 输入格式

输入只有一行两个整数，分别代表宗教数 $m$ 和房间数 $n$。

## 输出格式

输出一行一个整数代表答案。

```input1
2 3
```

```output1
6
```

## 样例说明

| 状态编号 | 一号房间 | 二号房间 | 三号房间 |
| :------: | :------: | :------: | :------: |
|   $1$   | 信仰 $1$ | 信仰 $1$ | 信仰 $1$ |
|   $2$   | 信仰 $1$ | 信仰 $1$ | 信仰 $2$ |
|   $3$   | 信仰 $1$ | 信仰 $2$ | 信仰 $2$ |
|   $4$   | 信仰 $2$ | 信仰 $1$ | 信仰 $1$ |
|   $5$   | 信仰 $2$ | 信仰 $2$ | 信仰 $2$ |
|   $6$   | 信仰 $2$ | 信仰 $2$ | 信仰 $1$ |

## 数据规模与约定

对于 $100\%$ 的数据，保证 $1 \le m \le 10^8$，$1 \le n \le 10^{12}$。