


## 题目描述
Tug of war is a very popular sport in Byteland. The rules are easy: two teams pull a rope in opposite directions. The annual Byteland tug of war charity is taking place, and a lot of contestants have signed up. As the fair play commissioner, your job is to divide the contestants into two teams, such that the game can go on for a long time.Since a total of 2N contestants have signed up, each team will consist of n contestants. The rope has n spots on the left side and n spots on the right side. The tug of war elite of Byteland are a picky bunch: each contestant has exactly one spot on the left side of the rope and one spot on the right side that he or she wants to use. Furthermore, you know the strength of each contestant. The organizer has now asked you the following: Given an integer k, is it possible to create two teams, such that each team has n contestants, each contestant uses a spot that he or she wants to use (of course no two contestants share a spot), and the sums of strengths of the two teams differ by at most  k
## 输入格式
The first line of input contains a positive integer n, specifying the number of spots on each side of the rope, and an integer K<=20N, specifying the maximum difference of teams' strengths. For simplicity, we number the contestants from 1 to 2N. Each of the following 2N lines describes one contestant: the i-th of these lines contains three positive integers Li, Ri and Si(1<=Li,Ri<=N,1<=Si<=20), which specify that contestant i has strength si and wants to use either spot li on the left side of the rope or spot Ri on the right side of the rope.
## 输出格式
In the first and only line of output your program should write either YES or NO, depending on whether it is possible to create two teams satisfying the requirements stated above.

```input1
4 1
1 1 1
2 1 2
2 2 8
1 2 2
3 3 5
3 3 2
4 4 1
4 4 2

```
```output1
YES
```

## 提示
Explanation to the example: In the first example we can assign contestants 1, 3, 6 and 7 to the left side (which results in a team of strength 1+8+2+1=12 and contestants 2, 4, 5 and 8 to the right side (which results in a team of strength 2+2+5+2=11. The difference of strengths between teams is 1.
求译文!请发至lydsy2012@163.com
## 题目来源
没有写明来源


