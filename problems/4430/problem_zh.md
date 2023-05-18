## 题目描述

Jaap, Jan, and Thijs are on a trip to the desert after having attended the ACM ICPC World Finals 2015 in Morocco. The trip included a camel ride, and after returning from the ride, their guide invited them to a big camel race in the evening. The camels they rode will also participate and it is customary to bet on the results of the race.  
One of the most interesting bets involves guessing the complete order in which the camels will finish the race. This bet offers the biggest return on your money, since it is also the one that is the hardest to get right.  
Jaap, Jan, and Thijs have already placed their bets, but the race will not start until an hour from now, so they are getting bored. They started wondering how many pairs of camels they have put in the same order. If camel $c$ is before camel $d$ on Jaap's, Jan's and Thijs' bet, it means that all three of them put $c$ and $d$ in the same order. Can you help them to calculate the number of pairs of camels for which this happened?

Jaap，Jan 和 Thijs 在摩洛哥参加完 ACM ICPC 2015 全球总决赛后去沙漠进行了一次旅行。旅行包括了骑骆驼。在骑完回来之后，他们的向导邀请他们在晚上去看一场盛大的骆驼赛跑。他们骑的骆驼也会参加，而赌比赛的结果是一个习惯。  
其中一个最有趣的赌涉及猜测完成比赛的骆驼的完整名单。这个赌可以为你赢得最多的钱，因为它也是最难猜对的。  
Jaap，Jan 和 Thijs 已经下了注，但比赛要在一个小时后才开始，所以他们觉得很无聊。他们开始想知道有多少对骆驼他们赌了同样的顺序。如果在他们三人的猜测名单中，骆驼 $c$ 在骆驼 $d$ 前，就意味着 $c$ 和 $d$ 在他们的名单中有相同的顺序。你能帮他们计算有多少对骆驼是这样的吗？

## 输入格式

The input consists of:  
one line with an integer $n$, the number of camels;  
one line with $n$ integers $a_1, \dots, a_n$,  Jaap's bet. Here $a_1$ is the camel in the first position of Jaap's bet, $a_2$ is the camel in the second position, and so on;  
one line with Jan's bet, in the same format as Jaap's bet;  
one line with Thijs' bet, in the same format as Jaap's bet.  
The camels are numbered $1, \dots, n$ . Each camel appears exactly once in each bet.

输入包括：  
第一行是一个整数 $n$，骆驼的数量。  
第二行有n个整数 $a_1, \dots, a_n$，是 Jaap 的下赌名单。$a_1$ 是名单中第一位，$a_2$ 是第二位，等等。  
第三行是 Jan 的名单，格式同上。  
第四行是 Thijs 的名单，格式同上。  
骆驼从 $1$ 到 $n$ 编号，每头骆驼在一份名单中只出现一次。

## 输出格式

Output the number of pairs of camels that appear in the same order in all $3$ bets.

输出在三份名单中同样顺序的骆驼有多少对。

```input1
3
3 2 1
1 2 3
1 2 3
```

```output1
0
```

```input2
4
2 3 1 4
2 1 4 3
2 4 3 1
```

```output2
3
```

## 数据规模与约定

对于 $100 \%$ 的数据，$2 \le n \le 200000$，$1 \le a_i \le n$。

