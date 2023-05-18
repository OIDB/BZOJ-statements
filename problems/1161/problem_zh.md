## 题目描述

HURRICANE 小组最近接到了一个搜索文本的任务，即从一个由数字构成的长文本中，匹配满足指定条件的子串。搜索的条件采用形如 $‘(0+10*1)*10*’$ 这样的正则表达式来描述。其中正则表达式的归纳定义如下：

$0, 1, \cdots , 9，0*, 1*, \cdots, 9*$ 是正则表达式；

如果 $A$ 和 $B$ 是正则表达式，则 $(A)，A+B，AB，(A)*$都是正则表达式；

只有按以上方法构造出来的表达式才是正则表达式。

其中，$A+B$ 表示「或者」关系，$AB$ 表示「连接」关系，$(A)*$ 表示 $A$ 的内容「重复」零次或者多次。

比如正则表达式 $(12+3)(4+5)6*$，就可以匹配以 $124, 125, 34, 35$ 之一开头，之后接零 $0$ 个或任意多个 $6$ 的字符串（例如字符串 $12566$）。正则表达式 $(1+0)*$ 可以匹配所有由 $0$ 和 $1$ 构成的字符串，或者是空串。如果一个正则表达式不能匹配空串，则称它是非空的。本题考虑的都是非空正则表达式。

如果在给定文本的某一个位置，存在一个以该位置结束的子串，能够被给定的非空正则表达式匹配，则称该位置是可匹配的。现在HURRICANE 小组接到的任务就是找出所有可匹配的位置。你能帮助他们完成这个任务么？

## 输入格式

第一行描述一个正则表达式，第二行为需要处理的文本。

第一行的正则表达式包括由一个空格分开的两个部分：

一个非负整数 $n$，表示我们所要考虑的数字集（即在正则表达式和文本中所出现的数字）是 $0, 1, \cdots, n–1$。

接下来是一个正则表达式，它由 $\{(, ), +, *\}$ 中的 $4$ 个符号和 $\{0, \cdots, n–1\}$ 中的数字构成，

第二行为一个由 $0$ 到 $n-1$ 之间数字构成的字符串，为需要处理的文本。

## 输出格式

输出只有一行，包括一些由空格分开的整数，按从小到大的顺序依次输出所需处理的文本中每一个可匹配的位置。

```input1
4 12333+33
312331
```

```output1
5
```

## 样例解释

需要处理的文本是 $312331$，其中只有第 $5$ 个字符所在的位置（下划线所在处）是可匹配的。这时正则表达式 $12333+33$ 中的 $33$ 可以与之匹配。

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 10$，表达式的长度不超过 $500$，文本长度不超过 $10^7$ 个字符。

共 $10$ 个测试点。有 $6$ 个测试点中的正则表达式不出现 $*$，其中有 $3$ 个测试点，正则表达式只由数字和 $+$ 构成。有一个测试点的待处理文本不超过 $10^6$ 个字符。该题有严格的时间限制，请尽量优化你的算法。