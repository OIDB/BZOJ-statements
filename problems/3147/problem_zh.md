## 题目描述

有 $n$ 位医生和 $m$ 位病人，其中某些医生需要给某些病人做手术，其中某些医生需要给某些病人做手术。为了避免医生的手直接接触到病人，医生在手术中必须佩带手套。然而，手套被使用后，内表面会沾染医生的汗液，外表面会沾染病人的血液。医生和病人都不愿意接触到其他人的汗液或血液。请你帮忙计算，最少使用多少副手套可以完成所有手术？值得注意的是：一副手套被当做一个整体，不可以拆成  「两只」  分别使用。此外，如果有必要，手套是可以  「翻过来」   使用的。

## 输入格式

输入的第一行包含一个正整数 $T$，表示该文件中含有  $T$ 组测试数据。

对于每组测试数据：第一行有三个正整数 $n,m,s$。表示有 $n$ 位医生（编号 $0$ 至 $n-1$ )，有 $m$ 位病人(编号 $0$ 至 $m-1$)，有 $s$ 场手术(编号 $0$ 至 $s-1$)。


随后 $s$ 行 ，按编号顺序描述每一场手术。每行有两个非负整数 $x,y$，表示 $x$ 号医生和 $y$ 号病人需要做一场手术。数据保证不会出现两场相同的手术。

## 输出格式

输出中应包含 $T$ 组测试数据的答案。

对于每一组答案：第一行包含一个正整数 $p$，表示你需要使用 $p$ 副手套(从字母 $a$ 开始顺序编号)。随后$s$ 行，你需要按时间顺序 描述每场手术安排，每场手术单独使用一行。对于一场手术，你需要先输出它的编号，随后输出它使用的手套数量 $k$ （必须是 $1$ 或  $2$ )，接下来以自内向外（从医生向病人）的顺序输出所有使用的 $k$ 副手套的编号 （字母），并用空格分隔。特别地，若某副手套在该次手术中是以「翻过来」的状态使用的，则用对应的大写字母来表示，否则用小写字母表示，详见样例。



```input1
2
2 2 4
0 1
0 0
1 0
1 1
3 2 3
0 1
1 0
2 1
```



```output1
2
1 2 a b
0 1 a 2 1 b
```

## 数据规模与约定

对于 $100\%$ 的数据，$T\le 10$，$n \le 10$，$m\le 10$，$s\le n\times m$。

## 题目来源

vfleaking提供spj
