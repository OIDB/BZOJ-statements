


## 题目描述
鼹鼠们在底下开凿了n个洞，由n-1条隧道连接，对于任意的i>1，第i个洞都会和第i/2（取下整）个洞间有一条隧
道，第i个洞内还有ci个食物能供最多ci只鼹鼠吃。一共有m只鼹鼠，第i只鼹鼠住在第pi个洞内，一天早晨，前k只
鼹鼠醒来了，而后n-k只鼹鼠均在睡觉，前k只鼹鼠就开始觅食，最终他们都会到达某一个洞，使得所有洞的ci均大
于等于该洞内醒着的鼹鼠个数，而且要求鼹鼠行动路径总长度最小。现对于所有的1<=k<=m，输出最小的鼹鼠行动
路径的总长度，保证一定存在某种合法方案。
## 输入格式
第一行两个数n,m（1<=n,m<=100000)，表示有n个洞，m只鼹鼠。
第二行n个整数ci表示第i个洞的食物数。
第三行m个整数pi表示第i只鼹鼠所在洞pi。
## 输出格式
输出一行m个整数，第i个整数表示当k=i时最小的鼹鼠行动路径总长度。

```input1
5 4
0 0 4 1 1
2 4 5 2

```
```output1
1 1 2 4
```

## 提示
没有写明提示
## 题目来源
没有写明来源

