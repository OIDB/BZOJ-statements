## 题目描述
某一天 WJMZBMR 在打 osu 但是他太弱逼了，有些地方完全靠运气。

我们来简化一下这个游戏的规则：

有 $n$ 次点击要做，成功了就是 $\text{o}$，失败了就是 $\text{x}$，分数是按 $comb$ 计算的，连续 $a$ 个 $comb$ 就有 $a\times a$ 分，$comb$ 就是极大的连续 $\text{o}$。

比如 $\text{ooxxxxooooxxx}$，分数就是 $2\times 2+4\times 4=4+16=20$。
1
Sevenkplus 闲的慌就看他打了一盘，有些地方跟运气无关要么是 $\text{o}$ 要么是 $\text{x}$ ，有些地方 $\text{o}$ 或者 $\text{x}$ 各有 $50\%$ 的可能性，用 $\text{?}$ 号来表示。

比如 $\text{oo?xx}$ 就是一个可能的输入。

那么 WJMZBMR 这场 osu 的期望得分是多少呢？

## 输入格式
第一行一个整数n，表示点击的个数；
接下来一个字符串，每个字符都是 $\text{o,x,?}$ 中的一个

## 输出格式
一行一个浮点数表示答案，并将其四舍五入到小数点后4位


```input1 
5
oo?xx
```

```output1
6.5000
```

```input2
4
????
```

```output2
4.1250
```

## 数据规模与约定

对于 $100%$ 的数据：$n\leq 300000$

## 提示
对于样例 $1$:

当 $\text{?}$ 是 $\text{o}$ 的话就是 $\text{oooxx}$，得分为 $9$

当 $\text{?}$ 是 $\text{x}$ 的话就是 $\text{ooxxx}$，得分为 $4$

期望则是：$\frac{9+4}{2}=6.5$

## 题目来源
我们都爱GYZ杯


