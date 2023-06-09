## 题目描述

给定 N 个点，求最小的球，使那些点都在球内或球上。

## 输入格式

多组数据： 第一行给出N的值点的坐标（均为实数）。所有坐标至多精确到小数点后第 4 位。一个 N=0 的数据标志着输入的结束。

## 输出格式

对于每一组 N>0 的数据仅输出一行，包括 4 个实数：第 1 个数是那个物体的半径，后 3 个给出其中心的坐标。每个实数精确到小数点后第 4 位（四舍五入）。设 Pi=3.14159265359。

```input1
2
1.7321 1.4142 2.2361
2.6458 1.7321 2.8284
0
```

```output1
0.5672 2.1890 1.5732 2.5322
```

## 提示

由于浮点运算会产生误差，请将绝对值小于 $10^{-7}$ 直接看成 0，以及把差的绝对值小于$10^{-7}$ 的两个数视为相等。

## 题目来源

鸣谢 a180285。

