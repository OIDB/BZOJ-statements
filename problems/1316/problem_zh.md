## 题目描述

一棵 $n$ 个点的带权有根树，有 $p$ 个询问，每次询问树中是否存在一条长度为 $k$ 的路径，如果是，输出 `Yes` 否输出 `No`. 

## 输入格式

第一行两个整数 $n, p$ 分别表示点的个数和询问的个数，   
接下来 $n-1$ 行每行三个数 $x, y, c$，表示有一条树边 $x \to y$，长度为 $c$，   
接下来 $p$ 行每行一个数 $k$，表示询问树中是否存在一条长度为 $k$ 的路径。

## 输出格式

输出有 $p$ 行，`Yes` 或 `No`. 

```input1
6 4
1 2 5
1 3 7
1 4 1
3 5 2
3 6 3
1
8
13
14
```

```output1
Yes
Yes
No
Yes
```

## 提示

$30\%$ 的数据，$n\le 100$，  
$100\%$ 的数据，$n\le 10000,p\le 100$，长度 $\le 1000000$，  
做完此题可看下 POJ 3237 Tree