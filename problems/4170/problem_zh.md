


## 题目描述
"若是万一琪露诺（俗称rhl）进行攻击，什么都好，冷静地回答她的问题来吸引她。对方表现出兴趣的话，那就慢
慢地反问。在她考虑答案的时候，趁机逃吧。就算是很简单的问题，她一定也答不上来。"               
 --《上古之魔书》
天空中出现了许多的北极光，这些北极光组成了一个长度为n的正整数数列a[i],远古之魔书上记载到：2个位置的g
raze值为两者位置差与数值差的和：
graze(x,y)=|x-y|+|a[x]-a[y]|。
要想破解天罚，就必须支持2种操作（k都是正整数）：
Modify x k：将第x个数的值修改为k。
Query x k：询问有几个i满足graze(x,i)<=k。
由于从前的天罚被圣王lmc破解了，所以rhl改进了她的法术，询问不仅要考虑当前数列，还要考虑任意历史版本，
即统计任意位置上出现过的任意数值与当前的a[x]的graze值<=k的对数。（某位置多次修改为同样的数值，按多次
统计）
## 输入格式
第1行两个整数n,q。分别表示数列长度和操作数。
第2行n个正整数，代表初始数列。
第3~q+2行每行一个操作。
N<=40000, 修改操作数<=60000, 询问操作数<=10000, Max{a[i]}(含修改)<=80000
## 输出格式
<span style="font-size:10.5pt;font-family:宋体;
mso-ascii-font-family:Consolas;mso-hansi-font-family:Consolas;mso-bidi-font-family:
Consolas;mso-font-kerning:1.0pt;mso-ansi-language:EN-US;mso-fareast-language:
ZH-CN;mso-bidi-language:AR-SA">对于每次询问操作，输出一个非负整数表示答案

```input1
3 5
2 4 3
Query 2 2
Modify 1 3
Query 2 2
Modify 1 2
Query 1 1

```

```output1
2
3
3
```

## 提示
没有写明提示
## 题目来源
没有写明来源


