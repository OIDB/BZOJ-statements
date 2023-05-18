


## 题目描述
在一片土地上有N个城市，通过N-1条无向边互相连接，形成一棵树的结构，相邻两个城市的距离为1，其中第i个城市的价值为value[i]。
不幸的是，这片土地常常发生地震，并且随着时代的发展，城市的价值也往往会发生变动。
接下来你需要在线处理M次操作：
0 x k 表示发生了一次地震，震中城市为x，影响范围为k，所有与x距离不超过k的城市都将受到影响，该次地震造成的经济损失为所有受影响城市的价值和。
1 x y 表示第x个城市的价值变成了y。
为了体现程序的在线性，操作中的x、y、k都需要异或你程序上一次的输出来解密，如果之前没有输出，则默认上一次的输出为0。
## 输入格式
第一行包含两个正整数N和M。
第二行包含N个正整数，第i个数表示value[i]。
接下来N-1行，每行包含两个正整数u、v，表示u和v之间有一条无向边。
接下来M行，每行包含三个数，表示M次操作。
## 输出格式
包含若干行，对于每个询问输出一行一个正整数表示答案。

```input1
8 1
1 10 100 1000 10000 100000 1000000 10000000
1 2
1 3
2 4
2 5
3 6
3 7
3 8
0 3 1

```

```output1
11100101
```

## 提示
1<=N,M<=100000
1<=u,v,x<=N
1<=value[i],y<=10000
0<=k<=N-1
## 题目来源
没有写明来源

