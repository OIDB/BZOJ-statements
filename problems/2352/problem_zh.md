

## 题目描述
在这个问题中，你需要设计一个简单的底层数据库。
简单的说，你需要写一个程序支持以下三个函数：
Init、CountPoint、InsertPoint。
下面是实现细节：
Init
C语言函数原型：void Init()。
Pascal语言函数原型：procedure Init。
没有输入参数，没有返回值，仅在程序开始时被调用一次。
CountPoint
C语言函数原型：int CountPoint(int Leftside, int Rightside)
Pascal语言函数原型：function CountPoint(Leftside,Rightside:longint):longint
两个参数分别为查询的左右边界，你应该返回之前有多少个点在当前给定左右边界内，在边界上的点视为在边界内。
参数类型：int/int(C/C++)，longint/longint(pascal)
返回值类型：int(C/C++)，longint(pascal)
InsertPoint
C语言函数原型：void InsertPoint(int Position)
Pascal语言函数原型：procedure InsertPoint(Position:longint)
输入参数为插入的点的坐标。
参数类型：int(C/C++)，longint(pascal)
没有返回值
本题已改成传统类型题,请自觉写在线算法
## 输入格式
## 输出格式

```input1
8
0 0
1 0 1
0 1
1 0 2
0 2
0 6
1 2 6
1 1 8

```
```output1
1
2
2
3
```

## 提示
没有写明提示
## 题目来源
没有写明来源


