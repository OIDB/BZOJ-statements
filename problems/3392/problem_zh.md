


## 题目描述
    奶牛们接到了寻找一种新型挤奶机的任务，为此它们准备依次经过N(1≤N≤50000)颗行星，在行星上进行交易．为了方便，奶牛们已经给可能出现的K(1≤K≤1000)种货物进行了由1到K的标号．由于这些行星都不是十分发达．没有流通的货币，所以在每个市场里都只能用固定的一种货物去换取另一种货物．    奶牛们带着一种上好的饲料从地球出发，希望进行最少的交易，最终得到所需要的机器．饲料的标号为1，所需要的机器的标号为K.如果任务无法完成，输出-1.
## 输入格式
    第1行是两个数字N和K.
    第2到N+1行，每行是两个数字Ai和Bi，表示第i颗行星愿意提供Ai为得到Bi．
## 输出格式
    第1行输出最小交换次数

```input1
6 5
1 3
3 2
2 3
3 1
2 5
5 4

```

```output1
4

奶牛们至少要交换4次，先用1去交换3，再用3去交换2，最后用2交换得到5．
```

## 提示
没有写明提示
## 题目来源
Silver

