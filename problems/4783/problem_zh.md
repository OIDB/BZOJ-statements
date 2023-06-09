## 题目描述

Always known for being quite tech-savy, Farmer John is testing out his new automated drone-mounted cow locator camera, which supposedly can take a picture of his field and automatically figure out the location of cows. Unfortunately, the camera does not include a very good algorithm for finding cows, so FJ needs your help developing a better one.

The overhead image of his farm taken by the camera is described by an $n \times n$ grid of characters, each in the range $A \ldots Z$, representing one of $26$ possible colors. Farmer John figures the best way to define a potential cow location (PCL) is as follows: A PCL is a rectangular sub-grid (possibly the entire image) with sides parallel to the image sides, not contained within any other PCL (so no smaller subset of a PCL is also a PCL). Furthermore, a PCL must satisfy the following property: focusing on just the contents of the rectangle and ignoring the rest of the image, exactly two colors must be present, one forming a contiguous region and one forming two or more contiguous regions.

```cpp
AAAAA
ABABA
AAABB
```

For example, a rectangle with contents

would constitute a PCL, since the A&#039;s form a single contiguous region and the B&#039;s form more than one contiguous region. The interpretation is a cow of color A with spots of color B.

A region is "contiguous" if you can traverse the entire region by moving repeatedly from one cell in the region to another cell in the region taking steps up, down, left, or right.

Given the image returned by FJ&#039;s camera, please count the number of PCLs.

## 输入格式

The first line of input contains $n$, the size of the grid.  
The next $n$ lines describe the image, each consisting of $n$ characters.

## 输出格式

Print a count of the number of PCLs in the image.




```input1
4
ABBC
BBBC
AABB
ABBC
```




```output1
2
```


## 样例解释

In this example, the two PCLs are the rectangles with contents

```cpp
ABB
BBB
AAB
ABB
```

and

```cpp
BC
BC
BB
BC
```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \leq n \leq 20$ 。

## 来源

Silver