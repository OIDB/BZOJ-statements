


## 题目描述
很久以前, 有一个小小的国度, 为了方便, 我们可以把它想象为一个大大的矩形, 矩形的左下角为(0, 0), 右上角为(w, h), 共有(w + 1) * (h + 1)个整点, 在本题中我们只考虑所有的整点．在这个国度里, 有n座山峰, 第i座位于整点(xi, yi)上, 现在我们需要选择一些整点来修建房子, 除了n座山峰以外还有(w + 1) * (h + 1) – n个可以修建房子的地方．
有些点修建房子风景会更加优美, 比如从这个点往北眺望可以看到一座山峰即你位于(x, y), 而存在一座位于(x, y + d)的山峰, 这样你就可以欣赏到山峰的美景, 东, 西, 南三个方向也同样如此．如果某个点上某个方向可以眺望到某座山峰, 那么我们称这座山峰为这个点的一个neighbour, 当然neighbour越多, 这个点修建房子风景会越优美．作为房地产开发公司的技术人员, 你的任务很简单, 统计在(w + 1) * (h + 1) – n 个点中neighbours总数为0, 1, 2, 3, 4的点的总数分别为多少
## 输入格式
输入文件第一行为3个正整数, w, h, n．
以下n行,每行有两个整数(xi, yi), 表示第i个山峰的位置(0 <= xi <= w, 0 <= yi <= h)．
## 输出格式
输出文件有5个数, 分别为neighbours总数为0, 1, 2, 3, 4的点的个数．

```input1
4 3 6
0 3
2 3
2 1
0 1
3 2
1 2

```

```output1
1 7 2 3 1
友情提示：共有(4 + 1) * (3 + 1) – 6 = 14个点, (4, 0)没有neighbour, (3, 1), (3, 3)有两个neighbours, (0, 2), (1, 1), (1, 3)有三个neighbours, (2, 2)有四个neighours, 其余点均为1个neighbour．
```

## 提示
100%的测试数据, N <= 500000, w, h <= 1000000000．
## 题目来源
没有写明来源

