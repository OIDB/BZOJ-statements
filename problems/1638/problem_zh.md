


## 题目描述
农场中,由于奶牛数量的迅速增长,通往奶牛宿舍的道路也出现了严重的交通拥堵问题.FJ打算找出最忙碌的道路来重点整治. 这个牧区包括一个由M (1 ≤ M ≤ 50,000)条单行道路(有向)组成的网络,以及 N (1 ≤ N ≤ 5,000)个交叉路口(编号为1..N),每一条道路连接两个不同的交叉路口.奶牛宿舍位于第N个路口.每一条道路都由编号较小的路口通向编号较大的路口.这样就可以避免网络中出现环.显而易见,所有道路都通向奶牛宿舍.而两个交叉路口可能由不止一条边连接. 在准备睡觉的时候,所有奶牛都从他们各自所在的交叉路口走向奶牛宿舍,奶牛只会在入度为0的路口,且所有入度为0的路口都会有奶牛. 帮助FJ找出最忙碌的道路,即计算所有路径中通过某条道路的最大次数.答案保证可以用32位整数存储. 
## 输入格式
第一行:两个用空格隔开的整数:N,M. 
第二行到第M+1行:每行两个用空格隔开的整数ai,bi,表示一条道路从ai到bi.
## 输出格式
第一行: 一个整数,表示所有路径中通过某条道路的最大次数. 

```input1
7 7
1 3
3 4
3 5
4 6
2 3
5 6
6 7

```
```output1
4
样例说明: 

    1   4
     \ / \
      3   6 -- 7
     / \ /
    2   5
通向奶牛宿舍的所有路径: 

    1 3 4 6 7
    1 3 5 6 7
    2 3 4 6 7
    2 3 5 6 7
```

## 提示
没有写明提示
## 题目来源
Silver

