## 题目描述

对 使用 $k$ 轮冒泡排序后有序的长度为 $n$ 的排列计数。

答案不取模，请注意实现方式。

对长度为 $n$ 的排列 $a$ 的第 $i$ 轮冒泡排序定义为：

```cpp
for(int j=1;j<=n-i;j++)
	if(a[j]>a[j+1])
		swap(a[j],a[j+1]);
```

## 输入格式

一行两个整数 $n,k$。

## 输出格式

一行一个整数表示你的答案。

```input1
8 5
```

```output1
10920
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n\leq 5\times 10^3$，$0<k<n$，答案的长度不超过 $2\times 10^4$。