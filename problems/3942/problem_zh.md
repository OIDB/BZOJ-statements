


## 题目描述
Farmer John has purchased a subscription to Good Hooveskeeping magazine for his cows, so they have plenty of material to read while waiting around in the barn during milking sessions. Unfortunately, the latest issue contains a rather inappropriate article on how to cook the perfect steak, which FJ would rather his cows not see (clearly, the magazine is in need of better editorial oversight).
FJ has taken all of the text from the magazine to create the string S of length at most 10^6 characters. From this, he would like to remove occurrences of a substring T to censor the inappropriate content. To do this, Farmer John finds the _first_ occurrence of T in S and deletes it. He then repeats the process again, deleting the first occurrence of T again, continuing until there are no more occurrences of T in S. Note that the deletion of one occurrence might create a new occurrence of T that didn't exist before.
Please help FJ determine the final contents of S after censoring is complete
有一个S串和一个T串，长度均小于1,000,000，设当前串为U串，然后从前往后枚举S串一个字符一个字符往U串里添加，若U串后缀为T，则去掉这个后缀继续流程。

```
## 输入格式
The first line will contain S. The second line will contain T. The length of T will be at most that of S, and all characters of S and T will be lower-case alphabet characters (in the range a..z).
```

## 输出格式
<h4 style="font-family: Raleway, 'Helvetica Neue', Helvetica, Arial, sans-serif; font-size: 14px;">The string S after all deletions are complete. It is guaranteed that S will not become empty during the deletion process.</h4>


```

```input1
whatthemomooofun
moo
```

```output1
whatthefun

```
## 提示
没有写明提示
## 题目来源
Silver
								
							
						
					
				
				
				
			
		
	
