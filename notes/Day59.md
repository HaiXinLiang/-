第十章 单调栈part02

● 503.下一个更大元素II 
● 42. 接雨水  

 详细布置 

 503.下一个更大元素II 

这道题和 739. 每日温度 几乎如出一辙，可以自己尝试做一做

https://programmercarl.com/0503.%E4%B8%8B%E4%B8%80%E4%B8%AA%E6%9B%B4%E5%A4%A7%E5%85%83%E7%B4%A0II.html  

视频：https://www.bilibili.com/video/BV15y4y1o7Dw

题目：https://leetcode.com/problems/next-greater-element-ii

看到题目的第一想法：直接看视频了。

实现过程中遇到哪些困难: 没想过循环可以用%，把for循环的list加倍，然后自变量i就用 i%size替代，妙

看完代码随想录之后的想法:

今日收获：

重点：

 42. 接雨水  

接雨水这道题目是 面试中特别高频的一道题，也是单调栈 应用的题目，大家好好做做。

建议是掌握 双指针 和单调栈，因为在面试中 写出单调栈可能 有点难度，但双指针思路更直接一些。

在时间紧张的情况有，能写出双指针法也是不错的，然后可以和面试官在慢慢讨论如何优化。 
https://programmercarl.com/0042.%E6%8E%A5%E9%9B%A8%E6%B0%B4.html  

视频：https://www.bilibili.com/video/BV1uD4y1u75P

题目：https://leetcode.com/problems/trapping-rain-water

看到题目的第一想法：直接看视频

实现过程中遇到哪些困难: 

看完代码随想录之后的想法:现在有很明显的可视化，单调栈的视图化

今日收获：完全没有想过原来单调递增栈，栈口元素就是凹槽点，哪里比较那元素就是凹槽点右边最大，而栈口第二个是凹槽的左边最大的元素！！

重点：
