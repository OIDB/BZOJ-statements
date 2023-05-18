


## 题目描述
体育课里一共有 N 个同学，学号分别为 1 到 N，JYY 的学号是 P。学号为 i
的同学的身高为hi。 
JYY的体育老师 KFC 有一个特殊排队方法： KFC 先让班里的N 个同学按照
学号从小到大的顺序，从左到右站成一排，然后从到队列的最左边（也就是第一
个学生面前）开始，一直向右走动到第 N-1 个学生面前；接着 KFC 再回到第一
个学生面前，继续开始向右走，就这样一共走动 N-1 次。每次当 KFC 走到第 i
个学生面前时，KFC 会比较一下队列里第i 个学生和第i+1 个学生的身高，如果
左边（第i 个）的学生比右边（第i+1）的学生高，那么KFC 就会交换这两个学
生在队列里的位置。 
最终，在 N-1 次走动全部结束之后，KFC 会选出队列最右边的一些学生去
搬桌子。自然的，JYY希望能够站在尽量靠左的位置来增加自己踢足球的机会。  
此外，JYY 还有一个绝招，那就是在 KFC 老师快走到自己面前的时候，开
始蹲下来系鞋带！如果 JYY 蹲下来系鞋带了，那么在这一次走动中，好说话的
KFC 老师就不会让 JYY和相邻的同学比较身高了， 自然也就不会让 JYY和相邻
的同学交换位置。 （只有 JYY最聪明会蹲下来系鞋带，其他同学都只会老老实实
的让KFC 老师比较身高） 
蹲下来系鞋带是很耗费体力的。为了留着体力踢足球，JYY最多只能蹲下 K
次。 
JYY想知道，按照怎样的下蹲策略可以使自己在队列里站的尽量靠左。 
我们用一个长度为 N-1的字符串来表示一个策略：如果字符串的第 i 个字符
是“+”，则表示在第 i 次走动时 JYY蹲下来系鞋带；如果第 i 个字符是“-”，则
表示JYY会老老实实的比较身高。
## 输入格式
第一行包含三个整数 N，P，K。
第二行包含 N 个整数，第 i 个整数表示 hi。
1  < =  P  < =  N  < =  10^5，0  < =  K  < =  N-1，1  < =  hi  < =  10^9
## 输出格式
第一行包含一个正整数，表示按照最优策略 JYY 可以排在的最
靠左的位置。 
输出文件的第二行包含一个长度为 N-1 的字符串，表示最佳策略。 
如果有多个最佳策略，JYY 希望知道字典序最大的策略。

```input1
10 7 7
8 3 5 4 5 7 4 2 1 3

```

```output1
3
----+++++
```

## 提示
没有写明提示
## 题目来源
By 佚名上传

