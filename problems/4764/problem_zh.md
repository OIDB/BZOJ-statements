## 题目描述

自从 WC 退役以来，大爷是越来越懒惰了。为了帮助他活动筋骨，也是受到了弹飞绵羊一题的启发，机房的小伙伴们决定齐心合力构造一个下面这样的序列。这个序列共有 $n$ 项，每项都代表了一个小伙伴的力量值，如果大爷落到了第 $i$ 个小伙伴的手里，那么第 $i$ 个小伙伴会把大爷弹到第 $i+a_i$ 个小伙伴手里，其中 $a_i$ 就是第 $i$ 个小伙伴的力量值，也就是序列的第 $i$ 项。然而，因为大爷太沉了，所以有些小伙伴不能撑到锻（you）炼（xi）结束，所以我们中途会替换一些小伙伴，也就是改变序列的某些项。而且，因为大爷太沉了，所以有些小伙伴不能把大爷扔向前方，而是会把大爷往反方向扔，也就是序列中的一些项会是负的（当然，也可能是零喽）。现在机智的大爷通过在空中的观察，已经知道小伙伴们的所有活动——即初始序列、所有更改操作，他想请你算一算，如果他在某时刻落到了某个位置，那么他会在几次弹起之后落到小伙伴序列之外（毕竟摔在地上还是蛮疼的）。

## 输入格式

第一行为两个整数 $n$ 和 $m$，代表序列长度和操作次数。  
第二行为 $n$ 个整数，代表初始的小伙伴序列。  
接下来有 $m$ 行，每行代表一个操作。  
如果这一行的第一个数是 $1$，代表该操作是一个询问操作，接下来一个数 $x$，代表询问此时大爷从 $x$ 处，经过几次弹起会摔在地上。如果永远不会摔在地上，请输出 `-1`。  
如果这一行的第一个数是 $2$，代表该操作是一个更改操作，接下来两个数 $x,y$，代表将序列的第 $x$ 项改为 $y$。  




```input1
3 19
1 1 1
1 1
1 2
1 3
2 1 2
1 1
1 2
1 3
2 3 -1
1 1
1 2
1 3
2 2 233
1 1
1 2
1 3
2 2 -233
1 1
1 2
1 3
```




```output1
3
2
1
2
2
1
-1
-1
-1
3
1
2
3
1
2
```



## 输出格式 

对于每次询问操作，输出弹起次数或 `-1`。

## 数据规模与约定

对于 $100\%$ 的数据，$n,m \le 2\times 10^5$，$|a_i| < n$。 

## 题目来源 

By YouSiki & GuoZZ