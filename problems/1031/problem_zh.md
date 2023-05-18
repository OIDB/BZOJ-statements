## 题目描述

喜欢钻研问题的 JS 同学，最近又迷上了对加密方法的思考。一天，他突然想出了一种他认为是终极的加密办法：把需要加密的信息排成一圈，显然，它们有很多种不同的读法。例如「JSOI07」，可以读作：

![](file://pic1.jpg)

$\text{JSOI07,SOI07J,OI07JS,I07JSO,07JSOI,7JSOI0}$。

把它们按照字符串的大小排序：$\text{07JSOI,7JSOI0,I07JSO,JSOI07,OI07JS,SOI07J}$。读出最后一列字符：$\text{I0O7SJ}$，就是加密后的字符串。

但是，如果想加密的字符串实在太长，你能写一个程序完成这个任务吗？

## 输入格式

输入文件包含一行，欲加密的字符串。注意字符串的内容不一定是字母、数字，也可以是符号等。

## 输出格式

输出一行，为加密后的字符串。


```input1
JSOI07
```


```output1
I0O7SJ
```

## 数据规模与约定

对于 $100\%$ 的数据，字符串的长度不超过 $10^5$。