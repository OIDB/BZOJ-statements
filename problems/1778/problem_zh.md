


## 题目描述
奶牛们建立了一个随机化的臭气炸弹来驱逐猪猡。猪猡的文明包含1到N (2 <= N <= 300)一共N个猪城。这些城市由M (1 <= M <= 44,850)条由两个不同端点A_j和B_j (1 <= A_j<= N; 1 <= B_j <= N)表示的双向道路连接。保证城市1至少连接一个其它的城市。一开始臭气弹会被放在城市1。每个小时（包括第一个小时），它有P/Q (1 <= P <=1,000,000; 1 <= Q <= 1,000,000)的概率污染它所在的城市。如果这个小时内它没有污染它所在的城市，那麽它随机地选择一条道路，在这个小时内沿着这条道路走到一个新的城市。可以离开这个城市的所有道路被选择的概率均等。因为这个臭气弹的随机的性质，奶牛们很困惑哪个城市最有可能被污染。给定一个猪猡文明的地图和臭气弹在每个小时内爆炸的概率。计算每个城市最终被污染的概率。如下例，假设这个猪猡文明有两个连接在一起的城市。臭气炸弹从城市1出发，每到一个城市，它都有1/2的概率爆炸。
1--2
可知下面这些路径是炸弹可能经过的路径（最后一个城市是臭气弹爆炸的城市）：
1: 1
2: 1-2
3: 1-2-1
4: 1-2-1-2
5: 1-2-1-2-1
...
要得到炸弹在城市1终止的概率，我们可以把上面的第1，第3，第5……条路径的概率加起来，（也就是上表奇数编号的路径）。上表中第k条路径的概率正好是(1/2)^k，也就是必须在前k-1个回合离开所在城市（每次的概率为1 - 1/2 = 1/2）并且留在最后一个城市（概率为1/2）。所以在城市1结束的概率可以表示为1/2 + (1/2)^3 + (1/2)^5 + ...。当我们无限地计算把这些项一个个加起来，我们最后会恰好得到2/3，也就是我们要求的概率，大约是0.666666667。这意味着最终停留在城市2的概率为1/3，大约为0.333333333。
## 输入格式
* 第1行: 四个由空格隔开的整数: N, M, P, 和 Q
* 第2到第M+1行: 第i+1行用两个由空格隔开的整数A_j和B_j表示一条道路。
## 输出格式
* 第1到第N行: 在第i行，用一个浮点数输出城市i被摧毁的概率。误差不超过10^-6的答桉会
被接受（注意这就是说你需要至少输出6位有效数字使得答桉有效）。

```input1
2 1 1 2
1 2

```

```output1
0.666666667
0.333333333
```

## 提示
没有写明提示
## 题目来源
Gold

