## 题目描述

排名系统通常要应付三种请求：上传一条新的得分记录、查询某个玩家的当前排名以及返回某个区段内的排名记录。

当某个玩家上传自己最新的得分记录时，他原有的得分记录会被删除。  

为了减轻服务器负担，在返回某个区段内的排名记录时，最多返回 $10$ 条记录。

## 输入格式

第一行是一个整数 $n$ 表示请求总数目。  

接下来 $n$ 行,每行包含了一个请求。请求的具体格式如下： 

+ `+Name Score`:上传最新得分记录。`Name` 表示玩家名字，由大写英文字母组成，不超过 $10$ 个字符。`Score` 为最多 $8$ 位的正整数。  

+ `?Name`:查询该玩家排名。该玩家的得分记录必定已经在前面上传。  

+ `?Index` 返回自第 `Index` 名开始的最多 $10$ 名玩家名字。`Index` 必定合法。

## 输出格式

对于 `?Name` 格式的请求，应输出一个整数表示该玩家当前的排名。

对于 `?Index` 格式的请求，应在一行中依次输出从第 `Index` 名开始的最多 $10$ 名玩家姓名，用一个空格分隔。

```input1
20
+ADAM 1000000
+BOB 1000000
+TOM 2000000
+CATHY 10000000
?TOM
?1
+DAM 100000
+BOB 1200000
+ADAM 900000
+FRANK 12340000
+LEO 9000000
+KAINE 9000000
+GRACE 8000000
+WALT 9000000
+SANDY 8000000
+MICK 9000000
+JACK 7320000
?2
?5
?KAINE
```

```output1
2
CATHY TOM ADAM BOB
CATHY LEO KAINE WALT MICK GRACE SANDY JACK TOM BOB
WALT MICK GRACE SANDY JACK TOM BOB ADAM DAM
4
```

## 样例说明

对于输入中的每个操作，解释如下。

```plain
+ADAM 1000000        加入ADAM的得分记录
+BOB 1000000         加入BOB的得分记录
+TOM 2000000         加入TOM的得分记录
+CATHY 10000000      加入CATHY的得分记录
?TOM                 输出TOM目前排名
?1                   目前有记录的玩家总数为4，因此应输出第1名到第4名。
+DAM 100000          加入DAM的得分记录
+BOB 1200000         更新BOB的得分记录
+ADAM 900000         更新ADAM的得分记录（即使比原来的差）
+FRANK 12340000      加入FRANK的得分记录
+LEO 9000000         加入LEO的得分记录
+KAINE 9000000       加入KAINE的得分记录
+GRACE 8000000       加入GRACE的得分记录
+WALT 9000000        加入WALT的得分记录
+SANDY 8000000       加入SANDY的得分记录
+MICK 9000000        加入MICK的得分记录
+JACK 7320000        加入JACK的得分记录
?2                   目前有记录的玩家总数为12，因此应输出第2名到第11名。
?5                   输出第5名到第13名。
?KAINE               输出KAINE的排名
```

## 数据规模与约定

对于 $100\%$ 的数据，$10\leq n\leq2.5\times10^5$。