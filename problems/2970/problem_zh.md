


## 题目描述
所有由节点0~K组成，且以0为根的不同的树，(注意共有K+1个节点)，如果放在一起，就会形成一个K-迷幻森林。我们记做F_{K}（当K取不同值时可以得到不同的迷幻森林）。
我们定义：一棵有根树的叶子，就是度为1的非根节点。
在这题中，我们研究的是一个迷幻森林中所有树的叶子个数Sum(F_{K})。
 
给出P, L, R, A。
在L ≤ K ≤ R中求：Sum(F_{K}) = A (mod P) 的不同的K有多少个。
 
## 输入格式
每个数据只有一行，为四个正整数P L R A。 其中P为质数。
## 输出格式
对每一个数据输出一行，即答案。

```input1【样例输入1】
3 1 3 1
【样例输入2】
13 1 10000 5

```

```output1【样例输出1】
2

【样例输出2】
641
【数据说明】
100%的数据满足 0 ≤ A < P ≤ 105；1 ≤ L ≤ R ≤ ­1018
 
```

## 提示
 题解：[JudgeOnline/upload/201604/sol.txt](/JudgeOnline/upload/201604/sol.txt)
## 题目来源
没有写明来源


