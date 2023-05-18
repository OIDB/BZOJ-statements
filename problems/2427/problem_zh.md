


## 题目描述
<span lang="RU" style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">现在我们的手头有<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">N<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">个软件，对于一个软件<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">i<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">，它要占用<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">W_{i}<span lang="RU" style="font-size:
12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">的磁盘空间，它的价值为<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">V_{i}<span lang="RU" style="font-size:
12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">。我们希望从中选择一些软件安装到一台磁盘容量为<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">M<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">计算机上，使得这些软件的价值尽可能大（即<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">V_{i}<span lang="RU" style="font-size:
12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">的和最大）。<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">

<span lang="RU" style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:
"Times New Roman";mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">但是现在有个问题：软件之间存在依赖关系，即软件<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">i<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">只有在安装了软件<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">j<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">（包括软件<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">j<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">的直接或间接依赖）的情况下才能正确工作（软件<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">i<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">依赖软件<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">j)<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">。幸运的是，一个软件最多依赖另外一个软件。如果一个软件不能正常工作，那么它能够发挥的作用为<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">0<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">。<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">

<span lang="RU" style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:
"Times New Roman";mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">我们现在知道了软件之间的依赖关系：软件<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">i<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">依赖软件<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">D_{i}<span lang="RU" style="font-size:
12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">。现在请你设计出一种方案，安装价值尽量大的软件。一个软件只能被安装一次，如果一个软件没有依赖则<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">D_{i}=0<span lang="RU" style="font-size:
12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">，这时只要这个软件安装了，它就能正常工作。<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">

## 输入格式
<span lang="RU" style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">第<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">1<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">行：<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">N, M<span lang="RU" style="font-size:12.0pt;
font-family:"Times New Roman";mso-fareast-font-family:宋体;color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA"> <span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA"> <span style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA">（<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">0<=N<=100, 0<=M<=500<span style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA">）<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">

<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";
mso-fareast-font-family:宋体;color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:ZH-CN;
mso-bidi-language:AR-SA">      <span lang="RU" style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">第<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">2<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">行：<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">W_{1}, W_{2}, ... W_{i}, ..., W_{n} <span style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:
"Times New Roman";mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:ZH-CN;
mso-bidi-language:AR-SA">（<span lang="RU" style="font-size:12.0pt;
font-family:"Times New Roman";mso-fareast-font-family:"Times New Roman";
color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">0<=W_{i}<=M<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
宋体;color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA"> <span style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA">）<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">

<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";
mso-fareast-font-family:宋体;color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:ZH-CN;
mso-bidi-language:AR-SA">      <span lang="RU" style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">第<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">3<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">行：<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">V_{1}, V_{2}, ..., V_{i}, ..., V_{n} <span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";
mso-fareast-font-family:宋体;color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:ZH-CN;
mso-bidi-language:AR-SA"> <span style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA">（<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">0<=Vi<=1000<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
宋体;color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA"> <span style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA">）<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">

<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";
mso-fareast-font-family:宋体;color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:ZH-CN;
mso-bidi-language:AR-SA">      <span lang="RU" style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">第<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">4<span lang="RU" style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">行：<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">D_{1}, D_{2}, ..., D_{i}, ..., D_{n}_{<span lang="RU" style="font-size:12.0pt;font-family:
"Times New Roman";mso-fareast-font-family:宋体;color:black;background:white;
mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:
ZH-CN;mso-bidi-language:AR-SA"> }<span style="font-size:12.0pt;
font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman";mso-bidi-font-family:"Times New Roman";color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA">（<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">0<=D_{i}<=N, D_{i}≠i<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
宋体;color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA"> <span style="font-size:12.0pt;font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
color:black;background:white;mso-shading:windowtext;mso-pattern:solid white;
mso-ansi-language:RU;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA">）<span lang="RU" style="font-size:12.0pt;font-family:"Times New Roman";mso-fareast-font-family:
"Times New Roman";color:black;background:white;mso-shading:windowtext;
mso-pattern:solid white;mso-ansi-language:RU;mso-fareast-language:RU;
mso-bidi-language:AR-SA">

## 输出格式
<span lang="RU" style="font-size:12.0pt;font-family:宋体;mso-bidi-font-family:宋体;color:black;
background:white;mso-shading:windowtext;mso-pattern:solid white;mso-ansi-language:
RU;mso-fareast-language:RU;mso-bidi-language:AR-SA">一个整数，代表最大价值。

```input1
3 10
5 5 6
2 3 4
0 1 1 

```

```output1
5
```

## 提示
没有写明提示
## 题目来源
Day2


