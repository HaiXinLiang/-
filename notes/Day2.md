2 第一章数组 
 
977.有序数组的平方 ，209.长度最小的子数组 ，59.螺旋矩阵II ，总结 

建议大家先独立做题，然后看视频讲解，然后看文章讲解，然后在重新做一遍题，把题目AC，最后整理成今日当天的博客

今天去office了，早上坐火车的时候先把视频看了。

拓展题目可以先不做

 详细布置

 977.有序数组的平方 

题目建议： 本题关键在于理解双指针思想 

题目链接：https://leetcode.cn/problems/squares-of-a-sorted-array/

文章讲解：https://programmercarl.com/0977.%E6%9C%89%E5%BA%8F%E6%95%B0%E7%BB%84%E7%9A%84%E5%B9%B3%E6%96%B9.html

视频讲解： https://www.bilibili.com/video/BV1QB4y1D7ep 

题目：https://leetcode.com/problems/squares-of-a-sorted-array/

看到题目的第一想法： 这是两边向中间靠的双指针。

实现过程中遇到哪些困难: 看完视频再做，完全没有什么困难。可能最大的困难是如果没有看视频，我会想到什么方法呢？会想到用双指针么？

看完代码随想录之后的想法:讲得很清晰。喜欢视频>喜欢文字 

今日收获：看完视频之后，自己可以写出来，不用debug都可以完成。

重点：

 209.长度最小的子数组

题目建议： 本题关键在于理解滑动窗口，这个滑动窗口看文字讲解 还挺难理解的，建议大家先看视频讲解。  拓展题目可以先不做。 

题目链接：https://leetcode.cn/problems/minimum-size-subarray-sum/
文章讲解：https://programmercarl.com/0209.%E9%95%BF%E5%BA%A6%E6%9C%80%E5%B0%8F%E7%9A%84%E5%AD%90%E6%95%B0%E7%BB%84.html
视频讲解：https://www.bilibili.com/video/BV1tZ4y1q7XE

题目：https://leetcode.com/problems/minimum-size-subarray-sum/

看到题目的第一想法： 

实现过程中遇到哪些困难: 开始做的时候，只是先把只要符合条件的就返回。然后运行了一下，发现问题，立刻想到用Math.min()

看完代码随想录之后的想法: 又用到双指针了。这是同向的双指针，看了视频后才深刻认识到，哪个应该作为快指针，哪个应该多为慢指针，如何取。

今日收获：又用到双指针！要多做题。双指针比两重for循环的效率高很多

重点：1. while(sum >= target) 而不是 if(sum >= target). 2. 不是判断完(sum >= target)后直接return，要快指针到数组最后，也就是要遍历数值所有元素。


 59.螺旋矩阵II

题目建议：  本题关键还是在转圈的逻辑，在二分搜索中提到的区间定义，在这里又用上了。 

题目链接：https://leetcode.cn/problems/spiral-matrix-ii/

文章讲解：https://programmercarl.com/0059.%E8%9E%BA%E6%97%8B%E7%9F%A9%E9%98%B5II.html

视频讲解：https://www.bilibili.com/video/BV1SL4y1N7mV/

题目：https://leetcode.com/problems/spiral-matrix-ii/

看到题目的第一想法： 很有意思的一道题目.

实现过程中遇到哪些困难: 引入offset变量后，debug很久才把code完成。 1.每到新的一层，如何定义开始值和结尾值？ 2.如果n%2 != 0,最后那数值的下标。

看完代码随想录之后的想法: 还好是看了视频再做，不然连基本原则都不会去定义。没想到二分搜索法中的区间定义可以这么运用。

今日收获：二分法的区间定义再次应用！

重点：新开每一层，得定义好开始值和结尾值！论test case的覆盖程度。没想到n<=5都没错，n=6会报错！

 **总结** (要留到周末了） 

题目建议：希望大家 也做一个自己 对数组专题的总结

文章链接：https://programmercarl.com/%E6%95%B0%E7%BB%84%E6%80%BB%E7%BB%93%E7%AF%87.html 
