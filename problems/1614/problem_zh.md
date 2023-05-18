


## 题目描述
Farmer John打算将电话线引到自己的农场，但电信公司并不打算为他提供免费服务。于是，FJ必须为此向电信公司支付一定的费用。 FJ的农场周围分布着N(1 <= N <= 1,000)根按1..N顺次编号的废弃的电话线杆，任意两根电话线杆间都没有电话线相连。一共P(1 <= P <= 10,000)对电话线杆间可以拉电话线，其余的那些由于隔得太远而无法被连接。 第i对电话线杆的两个端点分别为A_i、B_i，它们间的距离为 L_i (1 <= L_i <= 1,000,000)。数据中保证每对{A_i，B_i}最多只出现1次。编号为1的电话线杆已经接入了全国的电话网络，整个农场的电话线全都连到了编号为N的电话线杆上。也就是说，FJ的任务仅仅是找一条将1号和N号电话线杆连起来的路径，其余的电话线杆并不一定要连入电话网络。 经过谈判，电信公司最终同意免费为FJ连结K(0 <= K < N)对由FJ指定的电话线杆。对于此外的那些电话线，FJ需要为它们付的费用，等于其中最长的电话线的长度（每根电话线仅连结一对电话线杆）。如果需要连结的电话线杆不超过 K对，那么FJ的总支出为0。 请你计算一下，FJ最少需要在电话线上花多少钱。 
## 输入格式
* 第1行: 3个用空格隔开的整数：N，P，以及K
 * 第2..P+1行: 第i+1行为3个用空格隔开的整数：A_i，B_i，L_i
## 输出格式
* 第1行: 输出1个整数，为FJ在这项工程上的最小支出。如果任务不可能完成， 输出-1 

```input1
5 7 1
1 2 5
3 1 4
2 4 8
3 2 3
5 2 9
3 4 7
4 5 6
输入说明:
一共有5根废弃的电话线杆。电话线杆1不能直接与电话线杆4、5相连。电话
线杆5不能直接与电话线杆1、3相连。其余所有电话线杆间均可拉电话线。电信
公司可以免费为FJ连结一对电话线杆。

```
```output1
4

输出说明:

    FJ选择如下的连结方案：1->3；3->2；2->5，这3对电话线杆间需要的
电话线的长度分别为4、3、9。FJ让电信公司提供那条长度为9的电话线，于是，
他所需要购买的电话线的最大长度为4。
```

## 提示
没有写明提示
## 题目来源
Silver

