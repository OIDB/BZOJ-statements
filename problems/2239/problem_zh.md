


## 题目描述
When it's impossible to determine a winner after normal soccer play between two teams, a penalty shoot-out is used. During a penalty shoot-out, each of the teams takes k shots (each of those can either result in scoring a goal or not), and the team who scores the most goals is declared the winner. If both teams score an equal number of goals, we will assume in this problem that the game ends in a draw.
We will also assume that for each team there exists a number between 0 and 1, inclusive, denoting the skill level of that team, such that each penalty shot taken by that team results in a goal with probability equal to that number. You can assume that all shots are independent.
Your friend, an eager sports better, tells you that he knows that team 1 will win with probability p1%, team 2 will win with probability p2%, and the probability of a draw is pDraw%. You need to check if such a probability distribution is possible. In other words, can there exist two teams with valid skill levels such that those three outcomes would happen with the given probabilities?
Given ints p1, pDraw, p2 and k, return "YES" if such a distribution is possible, and "NO" otherwise (quotes for clarity only).
## Constraints|
:-:|
-p1, pDraw and p2 will be between 0 and 100, inclusive.
-p1, pDraw and p2 will sum up to 100.
-k will be between 1 and 5, inclusive.
## Constraints
-p1, pDraw and p2 will be between 0 and 100, inclusive.
-p1, pDraw and p2 will sum up to 100.
-k will be between 1 and 5, inclusive.
## 输入格式
## 输出格式

```input1
19 27 54 3 

```
```output1
NO
```

## 提示
没有写明提示
## 题目来源
没有写明来源


