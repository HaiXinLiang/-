第九章 动态规划part13
● 300.最长递增子序列 
● 674. 最长连续递增序列 
● 718. 最长重复子数组  

 详细布置  

 300.最长递增子序列 

今天开始正式子序列系列，本题是比较简单的，感受感受一下子序列题目的思路。 
视频讲解：https://www.bilibili.com/video/BV1ng411J7xP

https://programmercarl.com/0300.%E6%9C%80%E9%95%BF%E4%B8%8A%E5%8D%87%E5%AD%90%E5%BA%8F%E5%88%97.html

题目：https://leetcode.com/problems/longest-increasing-subsequence

看到题目的第一想法：直接看视频了。但是看了之后还是有三点比较懵懂。 1. 对dp[]数组的定义， 2. 递推公式 dp[i] = Math.max(dp[i], dp[j]+1) 3. 初始值得每个都是1

实现过程中遇到哪些困难: 1. 对dp[]数组的定义， 2. 递推公式 if(nums[j]<nums[i]) dp[i] = Math.max(dp[i], dp[j]+1) 3. 初始值得每个都是1

看完代码随想录之后的想法:

今日收获：

重点：初始值，应该考虑每个dp数组里面的初始值，而不是只考虑dp[0]或dp[1]

 674. 最长连续递增序列 

本题相对于昨天的动态规划：300.最长递增子序列 最大的区别在于“连续”。 先尝试自己做做，感受一下区别  
视频讲解：https://www.bilibili.com/video/BV1bD4y1778v

https://programmercarl.com/0674.%E6%9C%80%E9%95%BF%E8%BF%9E%E7%BB%AD%E9%80%92%E5%A2%9E%E5%BA%8F%E5%88%97.html  

题目：https://leetcode.com/problems/longest-continuous-increasing-subsequence

看到题目的第一想法：经过前面一题，这一题应该比较容易做出来

实现过程中遇到哪些困难: 忘了handle nums.length == 1的情况

看完代码随想录之后的想法: 这题的递推公式比起前一题，容易想出来

今日收获：

重点：

 718. 最长重复子数组 

稍有难度，要使用二维dp数组了
视频讲解：https://www.bilibili.com/video/BV178411H7hV

https://programmercarl.com/0718.%E6%9C%80%E9%95%BF%E9%87%8D%E5%A4%8D%E5%AD%90%E6%95%B0%E7%BB%84.html

题目：https://leetcode.com/problems/maximum-length-of-repeated-subarray

看到题目的第一想法：直接看视频，没有什么想法

实现过程中遇到哪些困难: 1.  //dp[i][j] 以nums1[i-1]和nums2[j-1]结尾最长重复子序列 2. int[][] dp = new int[nums1.length**+1**][nums2.length**+1**];

看完代码随想录之后的想法: dp数组的定义是以[i-1][j-1]这是因为方便初始化初始值

今日收获：

重点：
