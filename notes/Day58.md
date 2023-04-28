第十章 单调栈part01
 
● 739. 每日温度 
● 496.下一个更大元素 I  

 详细布置  

 739. 每日温度 

今天正式开始单调栈，这是单调栈一篇扫盲题目，也是经典题。

大家可以读题，思考暴力的解法，然后在看单调栈的解法。 就能感受出单调栈的巧妙

https://programmercarl.com/0739.%E6%AF%8F%E6%97%A5%E6%B8%A9%E5%BA%A6.html  

视频：https://www.bilibili.com/video/BV1my4y1Z7jj

题目：https://leetcode.com/problems/daily-temperatures/

看到题目的第一想法：直接看视频

实现过程中遇到哪些困难: 1. 虽然代码是比较简短，但是其实是分三种情况，拿遍历元素去和栈口比较 （> = <)，如果是单调递增栈就是 temperatures[i] > temperatures[dq.peek()]

看完代码随想录之后的想法:

今日收获：栈的应用。

重点：

 496.下一个更大元素 I 

本题和 739. 每日温度 看似差不多，其实 有加了点难度。

https://programmercarl.com/0496.%E4%B8%8B%E4%B8%80%E4%B8%AA%E6%9B%B4%E5%A4%A7%E5%85%83%E7%B4%A0I.html  

视频：https://www.bilibili.com/video/BV1jA411m7dX

题目：https://leetcode.com/problems/next-greater-element-i/

看到题目的第一想法：看了视频，和瞄了一下代码思想录的解答，但是对解法还是比较懵懂，最后冷静想了一下有了概念。

实现过程中遇到哪些困难: 主要解题思路是 1. nums1要用map装住。 2. 遍历nums2的时候，当和栈比较完后，就得去nums1 map那里查找下当前元素有没有在nums1里面出现。

看完代码随想录之后的想法: 

今日收获：

重点：
