第八章 贪心算法 part03

● 1005.K次取反后最大化的数组和 

● 134. 加油站

● 135. 分发糖果  

 详细布置 

 1005.K次取反后最大化的数组和  
本题简单一些，估计大家不用想着贪心 ，用自己直觉也会有思路。 

https://programmercarl.com/1005.K%E6%AC%A1%E5%8F%96%E5%8F%8D%E5%90%8E%E6%9C%80%E5%A4%A7%E5%8C%96%E7%9A%84%E6%95%B0%E7%BB%84%E5%92%8C.html  

视频：https://www.bilibili.com/video/BV138411G7LY

题目：https://leetcode.com/problems/maximize-sum-of-array-after-k-negations

看到题目的第一想法：自己尝试做了一下。

实现过程中遇到哪些困难: 没有想到直接用绝对值从大到小这样让数组进行排列。妙！

看完代码随想录之后的想法:

今日收获：用绝对值从大到小这样让数组进行排列
          IntStream.of(nums)
                .boxed()
                .sorted((x, y) -> Math.abs(y) - Math.abs(x))
                .mapToInt(Integer::intValue).toArray();

重点：


 134. 加油站 
本题有点难度，不太好想，推荐大家熟悉一下方法二 

https://programmercarl.com/0134.%E5%8A%A0%E6%B2%B9%E7%AB%99.html  

视频：https://www.bilibili.com/video/BV1jA411r7WX

题目：https://leetcode.com/problems/gas-station

看到题目的第一想法：看了视频。了解了原理

实现过程中遇到哪些困难: 自己试图去做，发现不知道怎么判断真的可以travel around the circuit once。发现少了totalSum的计算。

看完代码随想录之后的想法:

今日收获：

重点：

 135. 分发糖果 

本题涉及到一个思想，就是想处理好一边再处理另一边，不要两边想着一起兼顾，后面还会有题目用到这个思路 

https://programmercarl.com/0135.%E5%88%86%E5%8F%91%E7%B3%96%E6%9E%9C.html

视频：https://www.bilibili.com/video/BV1ev4y1r7wN

题目：https://leetcode.com/problems/candy/

看到题目的第一想法：看着视频写出来，但是运行结果不对。对照答案，看了半天，才发现是自己比较的时候用了candylist去比较，而不是ratingslist，真是不知道说什么好。。。自己思维不清晰呢。

实现过程中遇到哪些困难: 

看完代码随想录之后的想法:

今日收获：只是不合情理，但是合乎常理的一道题。

重点：1. 处理好一边，再处理一边，2. 拿左边比较右边的时候，要从后-》前遍历。
