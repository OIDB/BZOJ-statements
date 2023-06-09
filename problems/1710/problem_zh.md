## 题目描述
为了跟踪所有的牛，农夫 JOHN 在农场上装了一套自动系统。他给了每一个头牛一个电子牌号 当牛走过这个系统时，牛的名字将被自动读入。每一头牛的电子名字是一个长度为 $m$ 由 $n$ 个不同字母构成的字符串。很快，淘气的牛找到了系统的漏洞:它们可以倒着走过读码器。 一头名字为 `abcba` 不会导致任何问题，但是名为 `abcb` 的牛会变成两头牛（`abcb` 和 `bcba`）。农夫 JOHN 想改变牛的名字，使得牛的名字正读和反读都一样。例如，`abcb` 可以由在尾部添加 `a`。别的方法包 括在头上添加 `bcb`，得到 `bcbabcb` 或去掉 `a`，得到 `bcb`。JOHN 可以在任意位置添加或删除字母。因为名字是电子的，添加和删除字母都会有一定费用。添加和删除每一个字母都有一定的费用。对与一个牛的名字和所有添加或删除字母的费用，找出修改名字的最小的费用。空字符串也是一个合法的名字。
## 输入格式
* 第 $1$ 行：两个用空格分开的数， $n$ 和 $m$。
* 第 $2$ 行：$m$ 个字符，初始的牛的名字。
* 第 $3\dots n+2$ 行：每行含有一个字母和两个整数，分别是添加和删除这个字母的费用。
## 输出格式
一个整数， 改变现有名字的最小费用。

```input1
3 4
abcb
a 1000 1100
b 350 700
c 200 800
```
```output1
900
```
## 样例说明
输入解释：  
名字是 `abcb`，操作费用如下：
||添加|删除|
| :--: | :--: | :--: |
|a|1000|1100|
|b|350|700|
|c|200|800|

输出解释：  
在尾部添加 `a` 得到 `abcba` 的费用为 1000。删除头上的 `a`，得到 `bcb` 的费用为 1100。在头上添加 `bcb` 可以得到最小费用，350+200+350=900。
## 数据规模与约定
对于 $100\%$ 的数据，$1 \le m \le 2\times 10^3$，$1 \le n \le 26$，$0 \le$ 费用 $\le 10^4$。
## 题目来源
Gold