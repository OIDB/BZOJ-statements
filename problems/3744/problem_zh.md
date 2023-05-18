


## 题目描述
我早已习惯你不在身边，
人间四月天 寂寞断了弦。
回望身后蓝天，
跟再见说再见……
某天,蒟蒻Autumn发现了从 Gty的妹子树(bzoj3720) 上掉落下来了许多妹子,他发现
她们排成了一个序列,每个妹子有一个美丽度。
Bakser神犇与他打算研究一下这个妹子序列,于是Bakser神犇问道:"你知道区间
[l,r]中妹子们美丽度的逆序对数吗?"
蒟蒻Autumn只会离线乱搞啊……但是Bakser神犇说道:"强制在线。"
请你帮助一下Autumn吧。
给定一个正整数序列a,对于每次询问,输出al...ar中的逆序对数,强制在线。
## 输入格式
第一行包括一个整数n(1<=n<=50000),表示数列a中的元素数。
第二行包括n个整数a1...an(ai>0,保证ai在int内)。
接下来一行包括一个整数m(1<=m<=50000),表示询问的个数。
接下来m行,每行包括2个整数l、r(1<=l<=r<=n),表示询问al...ar中的逆序
对数(若ai>aj且i<j,则为一个逆序对)。
l,r要分别异或上一次询问的答案(lastans),最开始时lastans=0。
保证涉及的所有数在int内。
## 输出格式
对每个询问,单独输出一行,表示al...ar中的逆序对数。

```input1
4
1 4 2 3
1
2 4

```

```output1
2
```

## 提示
没有写明提示
## 题目来源
By Autumn

