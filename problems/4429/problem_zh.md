## 题目描述

Ellen is teaching elementary math to her students and the time for the final exam has come. The exam consists of $n$ questions. In each question the students have to add (+), subtract (−) or multiply (∗) a pair of numbers.  
Ellen has already chosen the $n$ pairs of numbers. All that remains is to decide for each pair which of the three possible operations the students should perform. To avoid students getting bored, Ellen wants to make sure that the $n$ correct answers to her exam are all different.  
Please help Ellen finish constructing the exam by automating this task.

Ellen 给她的学生教小学数学。期末考试已经来临了。考试有 $n$ 个题目，每一个题目学生们都要对一对数字进行加（+），减（-），乘（\*）运算。  
Ellen已经选好了 $n$ 对数。剩下的是决定学生们应该对每对数执行什么运算。为了不让学生们感到厌烦，Ellen 想确保 $n$ 个正确答案都不一样。  
请帮助 Ellen 自动化地构建考试。

## 输入格式

The input consists of:

* one line with one integer $n$, the number of pairs of numbers;
* $n$ lines each with two integers $a$ and $b$, a pair of numbers used.

输入包括：  
第一行是一个整数 $n$，表示共有 $n$ 道题目。  
接下来 $n$ 行每行有 $2$ 个整数 $a$ 和 $b$，表示每一题使用的整数。

## 输出格式

For each pair of numbers $(a, b)$ in the same order as in the input, output a line containing a valid equation. Each equation should consist of five parts: $a$, one of the three operators, $b$, an equals sign (=), and the result of the expression. All the $n$ expression results must be different.  
If there are multiple valid answers you may output any of them. If there is no valid answer, output a single line with the string “impossible” instead.
对于输入中的每一对 $(a,b)$，输出一行有效的方程。每一个方程应该包含5部分：$a$，`+`、`-`、`*` 中的一个运算符，$b$，`=`，答案。$n$ 个答案必须不同。  
如果有多个有效答案，你可以输出任意一个。如果没有答案，输出「impossible」。

```input1
4
1 5
3 3
4 5
-1 -6
```

```output1
1+5=6
3*3=9
4-5=-1
-1--6=5
```

```input2
4
-4 2
-4 2
-4 2
-4 2
```

```output2
impossible
```

## 数据范围与约定

对于 $100 \%$ 的数据，$1 \le n \le 2500$，$-10^6 \le a, b \le 10^6$。