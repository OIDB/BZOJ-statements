## 题目描述

Grant 是一个个体户老板，他经营的小店因为其丰富的优惠方案深受附近居民的青睐，生意红火。

小店的优惠方案十分简单有趣。Grant 规定：在一次消费过程中，如果您在本店购买了精制油的话，您购买香皂时就可以享受 $2.00$ 元/块的优惠价；如果您在本店购买了香皂的话，您购买可乐时就可以享受 $1.50$ 元/听的优惠价 $\dots\dots$ 诸如此类的优惠方案就是说：如果您在本店购买了商品 $a$ 的话，您就可以以 $p$ 元/件的优惠价格购买商品 $b$（购买的数量不限）。

有趣的是，你需要购买同样一些商品，由于不同的购买顺序，Grant 老板可能会叫你付不同数量的钱。比如你需要一块香皂（原价 $2.50$ 元）、一瓶精制油（原价 $10.00$ 元）、一听可乐（原价 $1.80$ 元），如果你按照可乐，精制油，香皂这样的顺序购买的话，Grant 老板会问你要 $13.80$ 元；而如果你按照精制油，香皂，可乐这样的顺序购买的话，您只需付 $13.50$ 元。

现在该村的居民请你编写一个程序，告诉你 Grant 小店商品的原价，所有优惠方案及所需的商品，计算至少需要花多少钱。不允许购买任何不需要的商品，即使这样做可能使花得钱更少。

## 输入格式

第一行为一个整数 $n$，表示 Grant 小店的商品种数。

接下来是 $n$ 行，其中第 $i+1$ 行由一个实数 $c_i$ 和一个整数 $m_i$ 组成，其间由一个空格分隔，分别表示第 $i$ 种商品的原价和所需数量。

第 $n+2$ 行又是一个整数 $k$，表示 Grant 小店的优惠方案总数。

接着 $k$ 行，每行有二个整数 $a,b$ 和一个实数 $p$，表示一种优惠方案，即如果您购买了商品 $a$，您就可以以 $p$ 元/件的优惠价格购买商品 $b,p$ 小于商品 $b$ 的原价。所有优惠方案的 $(a,b)$ 都是不同的。为了方便，Grant 不收分币，所以所有价格都不会出现分。

## 输出格式

只有一个实数，表示最少需要花多少钱。输出实数须保留两位小数。

```input1
4
10.00 1
1.80 1
3.00 0
2.50 2
2
1 4 2.00
4 2 1.50
```

```output1
15.50
```

## 数据范围与约定

$100\%$ 的数据满足：$1 \le n \le 50$，$0 < c_i \le 1000$，$0 \le m_i \le 100$，$1 \le a,b \le n$，$0 \le p < 1000$

