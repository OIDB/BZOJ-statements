


## 题目描述
我们给定一个整数集合A. 考虑一个非负整数集合A', 所有属于A' 的集合的数x满足当且仅当能被表示成一些属于A 的元素的和(数字可重复). 比如, 当 A = {2,5,7}, 属于A' 的数为: 0 (0个元素的和), 2, 4 (2  +  2) and 12 (5 + 7 or 7 + 5 or 2 + 2 + 2 + 2 + 2 + 2); 但是元素1和3不属于A'.
## 输入格式
第一行有一个整数n: 代表集合 A的元素个数, 1 <= n <= 5000. 接下来每行一个数a_{i}描述一个元素, 1 <= a_{i} <= 50000. A = {a_{1}, a_{2}, ..., a_{n}}, a_{1} < a_{2} < ... < a_{n}. 
接下来一个整数k, 1 <= k <= 10000. 每行一个0 到 1000000000, 分别代表b_{1}, b_{2}, ..., b_{k}.
## 输出格式
输出k行. 第i行打印<tt>TAK</tt>, 如果 b_{i} 属于A', 否则打印<tt>NIE</tt>. 
</divre>


```input1
3
2
5
7
6
0
1
4
12
3
2

```
```output1
TAK
NIE
TAK
TAK
NIE
TAK
 
```

## 提示
没有写明提示
## 题目来源
没有写明来源


