


## 题目描述
21YY年，夏。
时过境迁，小诚已是星际联邦（FederationofPlanets）太空防御理事会的技术顾问。去年联邦举行大选，新总统
刚刚宣誓就任。新政府的主要政策之一是对行政区域进行重新规划，将各个星球之间原有的行政关系精简。联邦有
N个星球，新的行政体系结构形如一个二叉树。联邦的行政中心为首都，其他所有星球分成至多两个区域，每个区
域内部又是同样的结构。在此番行政改革之前，每个星球驻扎着一支太空舰队。其中，第i个星球驻扎舰队的战斗
力是Fi。在行政改革的同时，太空防御理事会负责调整各个舰队的驻地，以符合军事条例中要求每个行政区域中心
驻扎的舰队是区域内战斗力最强舰队的规定。此外，根据军事条例，舰队调整驻地的方式只有一种，就是两个星球
的舰队交换驻防。现在，所有星球之间共有M条双向的星际航道。只有存在星际航道的两个星球才能进行舰队换防
。为了节省开支，理事会希望总的换防次数尽量少。早在年初，理事会就委托了小诚制定换防计划，但是小诚至今
还未完成任务。你能否帮助小诚，使他免于被解职的命运呢？
## 输入格式
第一行，两个整数N,M。
第二行，N个整数R1,R2,…,RN，由空格隔开。Ri表示星球i的直属上级星球编号。对于联邦首都，Ri用0表示。
第三行，N个互不相同的整数F1,F2,…,FN，由空格隔开。其中Fi表示当前驻扎在星球i的舰队的战斗力。
接下来M行，每行两个整数Xi,Yi，表示在星球Xi和星球Yi之间存在一条星际航道。
N<=12,M<=20
1 ≤ Fi ≤ 100。 输入数据保证星球之间的行政关系形成一个二叉
树， 任何两个星球之间至多有一条星际航道， 且星际航道不会出现自环。 数据保证有解。
## 输出格式
仅一行，一个整数，表示总换防次数的最小值。

```input1
4 4
0 1 2 3
1 2 3 4
1 2
1 4
2 3
1 3

```

```output1
2
```

## 提示
没有写明提示
## 题目来源
没有写明来源

