

## 题目描述
>There are two applications running on a multiprocessor machine. Each application i (i=1,2) consists of N procedures which are numbered from 1 to N and must be executed sequentially (in the order 1,...,N). A procedure will be identified by a pair (i,j), where i=1,2 identifies the application and 1≤j≤N represents the index of the procedure in the sequence of procedures of the application i. A procedure (i,j) can only be executed on the processor P(i,j) of the machine and its execution lasts for D(i,j) seconds. We want to schedule the execution of the procedures of the two applications over the processors of the machine in such a way that the time moment when the last procedure finishes its execution (from any of the two applications) is minimum; this time moment is called makespan. We consider that the two applications are available for scheduling starting from the time moment 0. The schedule needs to obey the following rules: 
>once the execution of a procedure (i,j) starts on the processor P(i,j), we cannot interrupt it until the execution of the procedure ends 
we cannot execute multiple procedures on the same processor at the same time, but we can execute multiple procedures in parallel on different processors 
the execution of the procedure (i,j) (2≤j≤N) starts either at the exact time moment tm when the procedure (i,j-1) finishes its execution or at any time moment after tm 
>if a procedure begins its execution at time moment tm, then it will finish its execution at the time moment tm+D(i,j) 

有两组任务，每组都有 $n$ 个程序，现在将这些任务放到一些处理器中处理，条件如下： 
- 任意一组任务必须按顺序完成，也就是必须先做完前 $i-1$ 个才能做第 $i$ 个。 
- 第 $i$ 组任务的第 $j$ 个程序只能在第 $p_{i,j}$ 个处理器上处理，耗时 $d_{i,j}$。 
- 一个处理器同一时间只能处理一个任务，并且不允许中断。 
求完成两组任务的最短时间。
## 输入格式
>Write a program that, given the information regarding the procedures of the two applications, computes the minimum makespan.
The first line of the input file contains the number T of test cases which are described next. The first line of a test case contains the number N (1≤N≤300) of procedures composing each of the two applications. Then, N lines follow, describing the first application. The j^{th} of these N lines contains two integers, separated by a blank: P(1,j) and D(1,j). After this, other N lines follow, describing the second application. The j^{th} of these N lines contains two integers, separated by a blank: P(2,j) and D(2,j). We have 1≤P(i,j)≤10 and 1≤D(i,j)≤15000 (i=1,2; 1≤j≤N). Notice that we may have P(i,j)=P(k,l) – this implies that the procedures (i,j) and (k,l) cannot be executed during overlapping time intervals (notice also that if i=k this would not matter, as the procedures of the same application must be executed sequentially).

第一行一个整数 $T$，代表数据组数。

对每组数据，第一行一个整数 $n$。

接下来 $n$ 行，第 $i$ 行两个整数表示 $p_{1,i},d_{1,i}$。

接下来 $n$ 行，第 $i$ 行两个整数表示 $p_{2,i},d_{2,i}$。

## 输出格式
>The output file must contain exactly T lines with a single number each – the minimum makespan for the corresponding test from the input file. These answers must be printed in the order in which the test cases are given in the input file (i.e. the i^{th} line of the output file contains the answer to the i^{th} test case from the input file).

对每组询问，输出答案。

```input1
2 
1 
2 6 
1 10 
3 
2 31 
2 18 
4 15 
2 26 
3 40 
5 16

```
```output1
10 
90
```

## 提示
$1\le n \le 300,1\le p_{i,j}\le 10,1\le d_{i,j}\le 1.5\times 10^4$
## 题目来源
Seerc2009

