


## 题目描述
有这样一种k*k位的十进制数，我们称它为“神经错乱数”，例如k=3时，100010001是这样的一种数字，因为：
1、首先按照从左往右，从上到下的顺序把数字写成一个正方形，像
123
456
789
所以将100010001写下来的话就会变成
100
010
001
2、对这个正方形进行a次横向的翻转操作，例如对
123
456
789
进行一次横向翻转操作将会变成
321
654
987
3、对这个正方形进行b次纵向的翻转操作，例如对
123
456
789
进行一次纵向翻转操作将会变成
789
456
123
4、对这个正方形进行2*c次向左旋转操作，例如对
123
456
789
进行一次向左旋转操作将会变成
369
258
147
5、对这个正方形进行2*d+1次向右旋转操作，例如对
123
456
789
进行一次向右翻转操作将会变成
741
852
963
6、只要你能选定一组正整数(a, b, c, d)，使得在最后的正方形中每一列的和都相同，那么原数就会被成为神经错乱数。
现在，我们想知道，和R位数相同并且大小不超过R的数当中，有多少个数是神经错乱数。
## 输入格式
输入一个正整数R。
数据保证R的位数不超过16位。
## 输出格式
输出一行，包括一个数字，表示有多少个神经错乱数满足要求。

```input1
3

```
```output1
4
```

## 提示
没有写明提示
## 题目来源
没有写明来源

