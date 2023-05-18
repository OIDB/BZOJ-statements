## 题目背景
这是一个很古老的游戏。用木棒在桌上拼出一个不成立的等式，移动且只移动一根木棒使得等式成立。现在轮到你了。

## 题目描述

![](file://pic1.jpg)

你只能移动用来构成数字的木棒，不能移动构成运算符 $(+,-,=)$ 的木棒，所以加号、减号、等号是不会改变的。移动前后，木棒构成的数字必须严格与图 $2$ 中的 $0 \to 9$ 相符。如果移动一根木棒可以使等式成立，则输出新的等式，否则输出 `No`。

![](file://pic2.jpg)

## 输入格式

输入数据要符合逻辑。字符串的长度小于等于 $1000$。

## 输出格式

如果有解，则输出正确的等式，格式与输入的格式相同（以 `#` 结尾，中间不能有分隔符，也不要加入多余字符）。此时输入数据保证解是唯一的。

如果无解，则输出 `No`。

```input1
1+1=3#
```
```output1
1+1=2#
```

```input2
1+1=3+5#
```
```output2
No
```

```input3
11+77=34#
```
```output3
17+17=34#
```