


## 题目描述
Bessie正在牛学院(cowllege)学习她最爱的课程：宏观经济学。为了准备她的毕业课题， 她要发表一篇关于国家之间汇率的研究报告。  为了使得她的报告更加生动，她将展示世界各地的巨无霸的价格(虽然她极其 讨厌这些不健康的垃圾食品)。通过给出巨无霸在某个国家的价格和一些国家 货币之间的汇率，Bessie想知道一个巨无霸在某个国家的最便宜的价格。  下面看个例子：  * 一个巨无霸在美国售价60美刀。  * 美刀对加拿大元的的汇率是0.2，也就是1美刀可以兑换0.2加拿大元  * 美刀对英镑的汇率是5.00，也就是1美刀可以兑换5.00英镑  * 英镑对加拿大元的汇率是0.5，也就是1英镑可以兑换0.5加拿大元  * 加拿大元对美刀的汇率是5.00，也就是1加拿大元可以兑换5.00美刀  Bessie想要找到在加拿大购买一个巨无霸最便宜的方式（通过货币的流通与兑换）。 以下有两种方式：  * 从美元直接兑换加拿大元，这样一个巨无霸价值   60 美刀 * 0.2 加拿大元 / 1 美刀 = 12 加拿大元。  * 从美元兑换成英镑，再有英镑兑换为加拿大元，这样一个巨无霸价值   60 美刀 * 5 英镑 / 1 美元 * 0.5 加元 / 1 英镑 = 150 加元。  Bessie会选择前一种兑换方式，这样她购买一个巨无霸可以只付12加元。  Bessie在研究N (1 <= N <= 2,000) 个国家，编号为1...N。她列出了M(1 <= M<= 25,000) 种兑换方式和相对应的汇率 e_ij (0.1 < e_ij <= 10)，表示国家i和j的货币 的兑换比例是e_ij(是单向的)。  给出一个实数V (1 <= V <= 1,000,000,000,000)，表示一个巨无霸在A国(1 <= A <= N)的售价。 你能够帮助她找到一种方式使得一个巨无霸在B国(1 <= B <= N; B != A)的售价尽可能少吗？ 如果售价没有最小值，输出0。  保证最终答案如果不是0，一定在1到10^15之间。  保证任何国家的货币可以兑换为任何另一个国家的货币。
## 输入格式
* 第1行： 5个空格分隔的数字： N, M, V, A, B  * 第2...M+1行： 三个空格分开的数字： i, j, e_ij
## 输出格式
* 第1行：如果不存在最小值，为0。否则是一个正数，和标准答案的差的绝对值不能大于10^-6。

```input1
3 4 60 1 2
1 2 0.2
1 3 5
3 2 0.5
2 1 5

```
```output1
12.00
```

## 提示
没有写明提示
## 题目来源
Gold鸣谢istream提供数据

