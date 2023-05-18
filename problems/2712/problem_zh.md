## 题目描述

棒球中一项最原始简单的技术参数就是「安打率」。  
所谓「安打」，就是指打击手把投手投出来的球，击出到界内，使打者本身能至少安全上到一垒的情形。  
由于只有队员跑回本垒才能得分，安打是得分的最重要的途径。  
因此，安打率对于打击手来说也是非常重要的数据。  
顾名思义，安打率为安打数与打数的比值。  
如果一名打击手在 $5$ 次打击中出现了 $1$ 次安打，那么他的安打率就是 $0.2$ 。  

 Uruto 是一位业余棒球爱好者。  
有一次，他在训练中看到了自己的安打率数据。  
他发现这个数据是一个被四舍五入到了 $n$ 位小数的一个值。  
 Uruto 想知道，他至少打击了多少次才有可能得到这样的安打率。  

## 输入格式

输入文件包含多个测试点。

每个测试点占一行，包含一个整数 $n$ 和一个浮点数 $r$ 。  
$r$ 是一个 $n$ 位小数，表示 Uruto 安打率的近似值。

## 输出格式

对于每个测试点，在单独的一行内输出一个整数，表示 Uruto 最小可能的打击次数。

```input1
2 0.33
3 0.316
```

```output1
3
19
```

## 样例说明

对于第一个测试点，如果 Uruto 只击打过 $2$ 次的话，那么他的安打率只能是 $0$ 、 $\frac{1}{2}$ 、 $1$ 中的一个，而其中的任何一个都不可能近似到 $2$ 位小数之后得到 $0.33$ 这样的值。  
如果他击打了 $3$ 次,出现了 $1$ 次安打，那么他的安打率就是 $\frac{1}{3}$ ，四舍五入到两位小数之后的值即为 $0.33$ 。

## 数据规模与约定

- 对于 $20\%$ 的数据，保证 答案在 $1000$ 以内。
- 对于 $100\%$ 的数据，保证 $0 < n \le 15$ ，测试点的数目在 $500$ 以内。
- 如果一个棒球运动员的安达率在 $30\%$ 以上，那么他就绝对是球队的栋梁了。出于这方面的考虑，保证所有的数据中 $0 \le r < 1$ 。

## 题目来源

applepi原创