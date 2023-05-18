## 题面描述：

约翰的 $ N $ 只奶牛非常兴奋，因为这是舞会之夜！她们穿上礼服和新鞋子，别上鲜花，她们要表演圆舞。

只有奶牛才能表演这种圆舞。

圆舞需要一些绳索和一个圆形的水池。奶牛们围在池边站好，顺时针顺序由 $1$ 到 $ N$ 编号．每只奶牛都面对水池，这样她就能看到其他的每一只奶牛。

为了跳这种圆舞，她们找了 $M$ 条绳索．若干只奶牛的蹄上握着绳索的一端，绳索沿顺时针方绕过水池，另一端则捆在另一些奶牛身上。

这样，一些奶牛就可以牵引另一些奶牛．有的奶牛可能握有很多绳索，也有的奶牛可能一条绳索都没有对于一只奶牛。

比如说贝茜，她的圆舞跳得是否成功，可以这样检验：沿着她牵引的绳索，找到她牵引的奶牛，再沿着这只奶牛牵引的绳索，又找到一只被牵引的奶牛，如此下去，若最终能回到贝茜，则她的圆舞跳得成功，因为这一个环上的奶牛可以逆时针牵引而跳起旋转的圜舞．如果这样的检验无法完成，那她的圆舞是不成功的。

如果两只成功跳圆舞的奶牛有绳索相连，那她们可以同属一个组合。

给出每一条绳索的描述，请找出，成功跳了圆舞的奶牛有多少个组合？

## 输入格式：
第 $1$ 行输入 $ N $ 和 $  M $ 

接下来 $ M$ 行每行两个整数 $A$  和 $B$ ，表示 $A $ 牵引着 $B$ .

## 输出格式：
一行一个数表示成功跳圆舞的奶牛组合数。

## 样例输入：
```
5 4
2 4
3 5
1 2
4 1
```

## 样例输出：

```
1
```

## 数据规模与约定：
对于 100\% 的数据 $2 \leq N \leq 10000$ ， $2 \leq M \leq 50000$。