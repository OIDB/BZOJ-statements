## 题目描述

有一天，小猫 rainbow 和 freda 来到了湘西张家界的天门山玉蟾宫，玉蟾宫宫主蓝兔盛情地款待了它们，并赐予它
们一片土地。

这片土地被分成 $ n\times m $ 个格子，每个格子里写着 ```R``` 或者 ```F```，```R``` 代表这块土地被赐予了rainbow，```F``` 代表这块土地被赐予了 freda。

现在 freda 要在这里卖萌……它要找一块矩形土地，要求这片土地都标着 ```F``` 并且面积最大。

但是 rainbow 和 freda 的 OI 水平都弱爆了，找不出这块土地，而蓝兔也想看 freda 卖萌（她显然是不会编程的……），所以它们决定，如果你找到的土地面积为 $ s $，它们每人给你 $ s $ 两银子。

## 输入格式

第一行两个整数 $ n,m $，表示矩形土地有 $ n $ 行 $ m $ 列。

接下来 $ n $ 行，每行 $ m $ 个用空格隔开的字符```F```或```R```，描述了矩形土地。

## 输出格式

输出一个整数，表示你能得到多少银子，即($ 3\times $ 最大```F```矩形土地面积)的值。

## 样例输入

```
5 6
R F F F F F
F F F F F F
R R R F F F
F F F F F F
F F F F F F
```

## 样例输出

```
45
```

## 数据规模与约定

对于 $50\%$ 的数据，$ 1\leq n,m\leq 200 $。

对于 $100\%$ 的数据，$ 1\leq n,m\leq 1\times 10^3 $。

## 题目来源

Poetize4

