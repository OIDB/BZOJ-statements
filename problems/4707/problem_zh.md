


## 题目描述
给出一个n，保证n=2^K（K为整数），和一个n*n的方阵Wi,j保证Wi,j=0(0≤i<n)且Wi,j=Wj,i(0≤i，j<n)求出一个
0，1…n一1的排列Pi，使得∑(Wpi-1,Pi)最小。但是这个排列还要满足一个特殊的条件：那就是对于所有的j(0≤J
≤K，从前往后分成2^(K-j)块，每块长度2^j，对于任意一块i，包含Pi2^^{j}，Pi2^^{j+1}，…，P(i+1)2^^{j-1}，这些数
的二进制第J位（最低位是第0位）都一样。比如3，2，0，1是满足条件的，而3，0，1，2不满足因为当j=l时，分
成的第一块3，0的第j=l位不相等，3的第1位是1而0的第1位是0。
## 输入格式
第一行一个K。从第二行开始，一个n×n的矩阵。
2<=k<=9,矩阵是关于主对角线对称的，每一项Wi,j在[0,1000000]
## 输出格式
第一行一个整数表示答案

```input1
2
0 7 2 1
7 0 4 3
2 4 0 5
1 3 5 0

```
```output1
13
【样例解释】
序列为1，0，3，2
```

## 提示
没有写明提示
## 题目来源
没有写明来源

