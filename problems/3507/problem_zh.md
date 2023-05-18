## 题目描述

几乎所有操作系统的命令行界面（CLI）中都支持文件名的通配符匹配以方便用户。最常见的通配符有两个，一个是星号（`*`），可以匹配 $0$ 个及以上的任意字符：另一个是问号（`?`），可以匹配恰好一个任意字符。

现在需要你编写一个程序，对于给定的文件名列表和一个包含通配符的字符串，判断哪些文件可以被匹配。

## 输入格式

第一行是一个由小写字母和上述通配符组成的字符串。

第二行包含一个整数 $n$，表示文件个数。

接下来 $n$ 行，每行为一个仅包含小写字母字符串，表示文件名列表。

## 输出格式

输出 $n$ 行，每行为 `YES` 或 `NO`，表示对应文件能否被通配符匹配。

```input1
*aca?ctc
6
acaacatctc
acatctc
aacacatctc
aggggcaacacctc
aggggcaacatctc
aggggcaacctct
```

```output1
YES
YES
YES
YES
YES
NO
```

## 提示

对于 $100\%$ 的数据：

- 字符串长度不超过 $10^5$。
- $1 \le n \le 100$。
- 通配符个数不超过 $10$。
