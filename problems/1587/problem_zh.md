## 题目描述
在一个美丽的秋天，丽丽每天都经过的花园小巷落满了树叶，她决定把树叶堆成 $k$ 堆，小巷是笔直的，共有 $n$ 片树叶（树叶排列也是笔直的），每片树叶都有一个重量值，并且每两片相邻的树叶之间的距离都是 $1$。现把所有的树叶按从左到右的顺序进行编号，编号为 $1\sim n$。丽丽移动每片树叶所消耗能量等于这片树叶的重量乘以移动的距离，丽丽决定分 $k$ 天完成，每天堆一堆，并且规定只能把树叶往左移动，因为丽丽每天都是从右往左经过小巷的。求丽丽完成任务所消耗的最少能量。

## 输入格式
* 第一行：两个用空格隔开的正整数： $n$ 和 $k$。
* 下面 $n$ 行：每行一个正整数，表示叶子的重量（第 $i+1$ 行表示第 $i$ 片树叶的重量）

## 输出格式
* 第一行：一个整数，表示把树叶堆成 $k$ 堆所消耗的最少体力。

```input1
5 2 
1
2
3
4
5
```
```output1
13
```

## 样例解释
$n$ 在 $(0,1001)$，$k$ 在 $(0,11)$，每片树叶的重量 $(0,1001)$。

## 数据规模与约定
对于 $100\%$ 的数据，$1\leq n \leq 1000$，$1\leq k \leq 10$。

约定所有树叶重量均不大于 $1000$。

