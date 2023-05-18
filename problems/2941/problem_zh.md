## 题目描述

在 Byteland 的安全局（BSA）里有职员和指挥官俩种等级。任一员工的资料都可在档案库里找到。在属于每个员工的文件夹中，都有一份 Signatures，Signatures 是其他的员工（职员或者指挥官）为他的忠诚所做的保证。每一新雇的职员都必须至少得到一份保证，但随着时间推移，保证人也会增加。BSA 最近发现，在他们的指挥官的圈子里已经有来自敌方Microsoftland的间谍的渗入。那么，BSA接下来就会雇佣其他的间谍作为他的职员由于这个间谍指挥官的保证或者其他雇佣间谍的保证。这些间谍有专门来自间谍员工的保证。

我们说一个职员的可信度值得怀疑，如果他没有获得任何一个不是间谍的指挥官的间接保证。即不存在这样的员工序列 $p_1,p_2,\cdots,p_k$，其中 $p_1$ 为一不是间谍的指挥官，对于员工 $p_i$，$p_i$ 为 $p_{i+1}$ 作保证。

如果我们假定一个指挥官是间谍，则使得他所担保的职员被怀疑是间谍。BSA 司令部急须知到这些职员的名单。

**举例**

指挥官：阿莉斯，Gregor
职员：鲍勃（阿莉斯保证），查利（鲍勃保证），戴维（鲍勃，并且查利保证），伊夫（阿莉斯和 Gregor 保证），夫兰克（伊夫保证），亨利（Gregor 和 Isabelle 保证），Isabelle（Gregor 和亨利保证）。

怀疑对象：

鲍勃，查利，戴维，亨利，Isabelle。

现在，你需要编写一个程序，计算确定被怀疑为间谍的职员的名单表。

## 输入格式

第一行为一正整数 $n$，，表示 BSA 的员工个数，员工从 $1$ 到 $n$ 标号。下面的 $n$ 行是职员担保的描述。

第 $i+1$ 行的数字是给第 $i$ 个员工作担保的员工编号，它是用单个空格隔开的数字序列。每行的第一个数字 $m_i$，表示为给第 $i$ 个员工作担保的其他员工的个数。接下来的 $m_i$ 个数字分别是这些员工的编号。员工的指挥官不需要任何人为其做担保。

## 输出格式

输出：

- 被怀疑为间谍的职员的编号，如果存在的话。连续输出，每行输出一个，升序。
- 仅输出一单词 `BRAK`，如果这样的职员不存在的话。

```input1
9
0
1 11 2
2 2 3
2 1 7
1 5
0
2 7 9
2 7 8
```

```output1
2
3
4
8
9
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n\le 500$。
