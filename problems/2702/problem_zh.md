## 题目描述

在这次金融危机爆发之前，小 L 就有预感。  
她准确地预测到了爆发地点以及扩散的式和速度。  
因此，金融危机爆发时，小 L 的很多好友都马上来找她帮忙，希望尽可能晚的遭到金融风暴的影响。  

为了简化问题，我们将地球变成二维平面（坐标值非负，最左与最右，最上与最下不可直接互达）。  
每个整点都为一个城市。  
在第 $0$ 时刻只有 $n$ 个金融中心爆发了金融风暴，第 $i$ 个金融中心是坐标 $（x_i,y_i）$。  
金融风暴扩散的方式是以金融中心为圆心做均匀的圆扩散。  
即世界上每个城市受到第 $i$ 个金融风暴影响的时间为这个城市与这场风暴中心 $（x_i,y_i）$ 的欧几里德距离。  
注意，地球外没有城市，金融危机也不会爆发到地球外面。  

小 L 希望你写个程序来帮帮她。  

现有 $t$ 个好友希望小 L 帮忙，因为各个人所在的不同地方以及国家大小原因。  
你需要告诉她与第 $i$ 个好友所在的 $（p_i,q_i）$ 横纵坐标距离不超过 $s_i$ 的所有城市 (即 $\max_{(a, b)} \{|a-p_i|,|b-q_i|\} \le s_i$ ) 中，最晚遭受金融风暴影响的城市开始爆发金融危机的时间（为严格定义，如果需要覆盖到地球外的区域，则输出 $-1$）。  

## 输入格式

第一行两个数，地图大小 $w,h$

第二行一个数 $n$ ,金融中心坐标

接下来 $n$ 行, $（x_i,y_i）$ $0 \le xi \le w,0 \le yi \le h$

第 $n+3$ 行一个数 $t$，为询问数

接下来 $t$ 行，每行三个数，$（p_i,q_i）$ 表示好友的坐标，$s_i$ 如题中描述意义。



## 输出格式

$t$ 行，每行一个数 $time$ 如题中描述。（保留 $3$ 位小数）

```input1
4 4
1
2 2
3
2 2 0
2 2 1
2 2 3
```

```output1
0.000
1.414
-1
```

## 数据规模与约定

- 对于 $20\%$ 的数据满足 $0 \le w,h \le 100$，$1 \le n,t \le 10^3$。
- 对于 $60\%$ 的数据满足 $1 \le t \le 2 \times 10^5$。
- 对于 $100\%$ 的数据满足 $0 \le w,h \le 10^3$，$1 \le n,t \le 10^6$。