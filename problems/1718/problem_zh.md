## 题目描述
In order to get from one of the $f\ (1 \le f \le 5\times 10^3)$ grazing fields (which are numbered $1\dots f$) to another field, Bessie and the rest of the herd are forced to cross near the Tree of Rotten Apples. The cows are now tired of often being forced to take a particular path and want to build some new paths so that they will always have a choice of at least two separate routes between any pair of fields. They currently have at least one route between each pair of fields and want to have at least two. Of course, they can only travel on Official Paths when they move from one field to another. Given a description of the current set of $r\ (f-1 \le r \le 10^4)$ paths that each connect exactly two different fields, determine the minimum number of new paths (each of which connects exactly two fields) that must be built so that there are at least two separate routes between any pair of fields. Routes are considered separate if they use none of the same paths, even if they visit the same intermediate field along the way. There might already be more than one paths between the same pair of fields, and you may also build a new path that connects the same fields as some other path.


为了从 $f$ 个草场中的一个走到另一个，贝茜和她的同伴们有时不得不路过一些她们讨厌的可怕的树。奶牛们已经厌倦了被迫走某一条路，所以她们想建一些新路，使每一对草场之间都会至少有两条相互分离的路径，这样她们就有多一些选择。每对草场之间已经有至少一条路径。给出所有 $r$ 条双向路的描述，每条路连接了两个不同的草场，请计算最少的新建道路的数量, 路径由若干道路首尾相连而成。两条路径相互分离，是指两条路径没有一条重合的道路。但是，两条分离的路径上可以有一些相同的草场。 对于同一对草场之间，可能已经有两条不同的道路，你也可以在它们之间再建一条道路，作为另一条不同的道路。
## 输入格式
* Line $1$: Two space-separated integers: $f$ and $r$.
* Lines $2\dots r+1$: Each line contains two space-separated integers which are the fields at the endpoints of some path.
* 第 $1$ 行输入 $f$ 和 $r$，接下来 $r$ 行，每行输入两个整数，表示两个草场，它们之间有一条道路。
## 输出格式
* Line $1$: A single integer that is the number of new paths that must be built.
* 最少的需要新建的道路数。
```input1
7 7
1 2
2 3
3 4
2 5
4 5
5 6
5 7
```
```output1
2
```
## 数据规模
对于 $100\%$ 的数据，$1\le f\le 5\times 10^3$，$f-1\le r\le 10^4$。
## 题目来源
Gold