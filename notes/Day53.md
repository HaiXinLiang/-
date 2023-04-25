第九章 动态规划part14
● 1143.最长公共子序列 
● 1035.不相交的线   
● 53. 最大子序和  动态规划 

 详细布置 

 1143.最长公共子序列 

体会一下本题和 718. 最长重复子数组 的区别  
视频讲解：https://www.bilibili.com/video/BV1ye4y1L7CQ
https://programmercarl.com/1143.%E6%9C%80%E9%95%BF%E5%85%AC%E5%85%B1%E5%AD%90%E5%BA%8F%E5%88%97.html

题目：https://leetcode.com/problems/longest-common-subsequence

看到题目的第一想法：又是两个数组，所以还是二维数组

实现过程中遇到哪些困难: 跟最长重复子数组不同的是递推公式 不仅仅要求两数组的某一数值相同的时候，还要求两数组的某一数值不相同的时候

看完代码随想录之后的想法:

今日收获：

重点：A subsequence of a string is a new string generated from the original string with some characters (can be none) deleted **without changing the relative order** of the remaining characters.

 1035.不相交的线 

其实本题和 1143.最长公共子序列 是一模一样的，大家尝试自己做一做。
视频讲解：https://www.bilibili.com/video/BV1h84y1x7MP
https://programmercarl.com/1035.%E4%B8%8D%E7%9B%B8%E4%BA%A4%E7%9A%84%E7%BA%BF.html

题目：https://leetcode.com/problems/uncrossed-lines

看到题目的第一想法：没有想过这题跟前面一题是一模一样的，战战兢兢地把前一题的答案抄了一遍，通过了。然后又仔细的分别读了这两题的题目。

实现过程中遇到哪些困难: 直接看视频

看完代码随想录之后的想法:

今日收获：

重点：

 53. 最大子序和 

这道题我们用贪心做过，这次 再用dp来做一遍 
视频讲解：https://www.bilibili.com/video/BV19V4y1F7b5
https://programmercarl.com/0053.%E6%9C%80%E5%A4%A7%E5%AD%90%E5%BA%8F%E5%92%8C%EF%BC%88%E5%8A%A8%E6%80%81%E8%A7%84%E5%88%92%EF%BC%89.html

题目：https://leetcode.com/problems/maximum-subarray

看到题目的第一想法：看视频了。

实现过程中遇到哪些困难: 最重要的是明确dp数组的定义 //dp[i] 以i结尾nums[i]的最大连续子序列和

看完代码随想录之后的想法:

今日收获：

重点：
