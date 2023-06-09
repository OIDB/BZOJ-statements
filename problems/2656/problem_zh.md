## 题目描述

小白和小蓝在一起上数学课，下课后老师留了一道作业，求下面这个数列的通项公式：

$$
a_0=0,a_1=1,a_{2i}=a_{i},a_{2i+1}=a_{i}+a_{i+1}
$$

小白作为一个数学爱好者，很快就计算出了这个数列的通项公式。于是，小白告诉小蓝自己已经做出来了，
但为了防止小蓝抄作业，小白并不想把公式公布出来。于是小白为了向小蓝证明自己的确做出来了此题以达到
其炫耀的目的，想出了一个绝妙的方法：即让小蓝说一个正整数 $n$，小白则说出 $a_n$ 的值，如果当 $n$ 很大时小白仍能很快的说出正确答案，这就说明小白的确得到了公式。但这个方法有一个很大的漏洞：小蓝自己不会做，没法验证小白的答案是否正确。作为小蓝的好友，你能帮帮小蓝吗？

## 输入格式

输入文件第一行有且只有一个正整数 $T$，表示测试数据的组数。

接下来 $T$ 行，每行一个整数 $n$。

## 输出格式

对于每组数据：输出一行一个整数代表 $a_n$。

## 样例输入

```plain
3
1
3
10
```

## 样例输出

```plain
1
2
3
```

## 数据规模与约定

$T\le 20,N\le10^{100}$。

