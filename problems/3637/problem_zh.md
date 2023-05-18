


## 题目描述
You are given a tree (an acyclic undirected connected graph) with n nodes. The tree nodes are numbered from 1 to n. 
Each node has a color, white or black. All the nodes are black initially.
We will ask you to perfrom some instructions of the following form:
<ul type="disc">

0 u : ask for how many nodes are connected to u, two nodes are connected iff all the node on the path from u to v (inclusive u and v) have a same color. 
1 u : toggle the color of u(that is, from black to white, or from white to black). 
## 输入格式
The first line contains a number n denoted how many nodes in the tree(1 ≤ n ≤ 10^{5}). The next n - 1 lines, each line has two numbers (u,  v) describe a edge of the tree(1 ≤ u,  v ≤ n). The next line contains a number m denoted how many operations we are going to process(1 ≤ m ≤ 10^{5}). The next m lines, each line describe a operation (t,  u) as we mentioned above(0 ≤ t ≤ 1, 1 ≤ u ≤ n).
## 输出格式
 
For each query operation, output the corresponding result.

```input1
5
1 2
1 3
1 4
1 5
3
0 1
1 1
0 1

```
```output1
5
1
```

## 提示
没有写明提示
## 题目来源
By xiaodao


