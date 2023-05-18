

## 题目描述
考虑一个非递减的整数序列 $S_1,....S_{n+1}(Si\leq Si+1 , 1\leq i\leq n)$。

序列 $M_1...M_n$ 是定义在序列 $S$ 的基础上，关系式为 $M_i=( S_i + S_{i+1} ) )/2, 1\leq i\leq n$,

序列 $M$ 叫做序列 $S$ 的平均数序列。例如序列 $1,2,2,4$ 的平均数序列为 $1.5,2,3$ .注意到平均数序列中的元素可能为小数。但是本题的任务只是处理平均数序列都为整数的情况。

给出一个 $n$ 个数字的非递减的整数序列 $M_1,M_2...M_n$.请你计算出：序列{S},$S_1...S_{n+1} $的平均序列 $M_1,...,M_n$。

求满足以上条件的序列S的总个数。

任务：
* 从标准输入文件中读入一个非递减的整数序列。

* 计算出平均序列是给出序列的整数序列的总个数。

* 把计算结果写到标准输出文件中。

## 输入格式

输入文件的第一行包含一个整数n.接下来的n行包含了这个给出的整数序列M1,..,Mn.

第 $i+1$ 行包含一个整数 $M_i$.

## 输出格式

输出文件仅一行，即所求答案。

```input1
3
2
5
9	

```
```output1
4
```

## 数据规模与约定

对于50%的数据:

$n\leq 1000,0\leq M_i\leq 20000$.

对于100%的数据:

$2\leq n\leq 5\times 10^6$

$1\leq M_i\leq 10^9$

## 提示
本题一共存在4种序列， 他们的平均数序列都是2,3,9。这四种序列如下：
* 2,2,8,10
* 1,3,7,11
* 0,4,6,12
*-1,5,5,13
## 题目来源
没有写明来源

