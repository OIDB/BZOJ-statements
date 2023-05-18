

## 题目描述
你要用 $n$ 个积木拼成一个塔，第 $i$ 块积木长度是 $a_i$。

给定 $D$，积木 $i$ 能搭在积木 $j$ 上面，当且仅当 $a_i-a_j\le D$。

求合法的搭积木方案数对 $998244353$ 取模后的结果。
## 输入格式
第一行两个整数 $n,D$。表示积木的数量和搭建的限制。

第二行 $n$ 个整数 $a_i$，表示每块积木的长度。
## 输出格式
一行一个整数，表示搭积木的方案数对 $998244353$ 取模后的结果。

```input1
4 1
1 2 3 100
```
```output1
4
```
## 提示
样例解释：最后一个积木只能在下面，考虑前 $3$ 个积木，$(1,2,3),(2,3,1),(3,1,2),(3,2,1)$ 都是合法的。

对于$100\%$ 的数据，满足 $1\le n\le 7\times 10^5$。
## 题目来源
没有写明来源