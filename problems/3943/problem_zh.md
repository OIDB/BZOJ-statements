


## 题目描述
Bessie and her friends are playing hoofball in the annual Superbull championship, and Farmer John is
 in charge of making the tournament as exciting as possible. A total of N (1 <= N <= 2000) teams are
 playing in the Superbull. Each team is assigned a distinct integer team ID in the range 1...2^30-1 
to distinguish it from the other teams. The Superbull is an elimination tournament -- after every ga
me, Farmer John chooses which team to eliminate from the Superbull, and the eliminated team can no l
onger play in any more games. The Superbull ends when only one team remains.Farmer John notices a ve
ry unusual property about the scores in matches! In any game, the combined score of the two teams al
ways ends up being the bitwise exclusive OR (XOR) of the two team IDs. For example, if teams 12 and 
20 were to play, then 24 points would be scored in that game, since 01100 XOR 10100 = 11000.Farmer J
ohn believes that the more points are scored in a game, the more exciting the game is. Because of th
is, he wants to choose a series of games to be played such that the total number of points scored in
 the Superbull is maximized. Please help Farmer John organize the matches.
贝西和她的朋友们在参加一年一度的“犇”(足)球锦标赛。FJ的任务是让这场锦标赛尽可能地好看。一共有N支球
队参加这场比赛，每支球队都有一个特有的取值在1-230-1之间的整数编号(即：所有球队编号各不相同)。“犇”
锦标赛是一个淘汰赛制的比赛——每场比赛过后，FJ选择一支球队淘汰，淘汰了的球队将不能再参加比赛。锦标赛
在只有一支球队留下的时候就结束了。FJ发现了一个神奇的规律：在任意一场比赛中，这场比赛的得分是参加比赛
两队的编号的异或(Xor)值。例如：编号为12的队伍和编号为20的队伍之间的比赛的得分是24分，因为 12(01100) 
Xor 20(10100) = 24(11000)。FJ相信比赛的得分越高，比赛就越好看，因此，他希望安排一个比赛顺序，使得所
有比赛的得分和最高。请帮助FJ决定比赛的顺序
## 输入格式
The first line contains the single integer N. The following N lines contain the N team IDs.
第一行包含一个整数N接下来的N行包含N个整数，第i个整数代表第i支队伍的编号, 1<=N<=2000
## 输出格式
<h4 style="font-family: Raleway, 'Helvetica Neue', Helvetica, Arial, sans-serif; font-size: 14px;">

Output the maximum possible number of points that can be scored in the Superbull.
一行，一个整数，表示锦标赛的所有比赛的得分的最大值
</h4>


```input1
4
3
6
9
10

```

```output1
37
```

## 提示
样例解释：
FJ先让编号为3和编号为9的队伍进行比赛，然后让编号为9的队伍赢得比赛(淘汰编号为6的队伍)，现在
剩下了编号为6910的队伍。然后他让编号为6和编号为9的队伍比赛，然后让编号为6的队伍赢得比赛。现在编号为6
10的队伍留了下来最后让编号为6和编号为10的队伍比赛，让编号为10的队伍赢得比赛。所有比赛的得分和就是：(
3Xor9)+(6Xor9)+(6Xor10)=10+15+12=37
## 题目来源
Silver


