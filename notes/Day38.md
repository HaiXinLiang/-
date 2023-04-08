第九章 动态规划part01

● 理论基础 

● 509. 斐波那契数 

● 70. 爬楼梯 

● 746. 使用最小花费爬楼梯 

 详细布置 

今天正式开始动态规划！

 理论基础 

无论大家之前对动态规划学到什么程度，一定要先看 我讲的 动态规划理论基础。 

如果没做过动态规划的题目，看我讲的理论基础，会有感觉 是不是简单题想复杂了？ 

其实并没有，我讲的理论基础内容，在动规章节所有题目都有运用，所以很重要！  

如果做过动态规划题目的录友，看我的理论基础 就会感同身受了。

https://programmercarl.com/%E5%8A%A8%E6%80%81%E8%A7%84%E5%88%92%E7%90%86%E8%AE%BA%E5%9F%BA%E7%A1%80.html 

视频：https://www.bilibili.com/video/BV13Q4y197Wg  

今日收获：能比较规范的学习动态规划编程比较兴奋。 貌似之前没有做过动态规划。

重点：1. 明白dp[]数组及下标的含义 2. 推论公式 3. 确定初始值 4. 确定遍历循序 5 打印dp[]函数。

 509. 斐波那契数 

很简单的动规入门题，但简单题使用来掌握方法论的，还是要有动规五部曲来分析。

https://programmercarl.com/0509.%E6%96%90%E6%B3%A2%E9%82%A3%E5%A5%91%E6%95%B0.html  

视频：https://www.bilibili.com/video/BV1f5411K7mo  

题目：https://leetcode.com/problems/fibonacci-number

看到题目的第一想法：听听Carl老师讲课，从一开始规范递归学习。

实现过程中遇到哪些困难: 一开始，还没有明白问什么是直接return dp[n]了。那是没有深刻理解dp[]组合及下标的含义

看完代码随想录之后的想法:

今日收获：

重点：

 70. 爬楼梯   

本题大家先自己想一想， 之后会发现，和 斐波那契数 有点关系。

https://programmercarl.com/0070.%E7%88%AC%E6%A5%BC%E6%A2%AF.html  

视频：https://www.bilibili.com/video/BV17h411h7UH  

题目：https://leetcode.com/problems/climbing-stairs

看到题目的第一想法：

实现过程中遇到哪些困难: 1. 一开始没有想出递推公式， 是看了视频后才知道的。
2. 也不明白为什么 int[] dp = dp[**n+1**] 而不是 int[] dp = dp[**n**]。 后来debug明白了。其实也是对dp组合和下标含义不是太理解。

看完代码随想录之后的想法:

今日收获：

重点：

 746. 使用最小花费爬楼梯 

这道题目力扣改了题目描述了，现在的题目描述清晰很多，相当于明确说 第一步是不用花费的。 

更改题目描述之后，相当于是 文章中 「拓展」的解法 

https://programmercarl.com/0746.%E4%BD%BF%E7%94%A8%E6%9C%80%E5%B0%8F%E8%8A%B1%E8%B4%B9%E7%88%AC%E6%A5%BC%E6%A2%AF.html   

视频讲解：https://www.bilibili.com/video/BV16G411c7yZ 

题目：https://leetcode.com/problems/min-cost-climbing-stairs/

看到题目的第一想法：没能做出来，也没有想到推理公式。看了视频后，本来不是太理解，慢慢做出了后，再理解一番。

实现过程中遇到哪些困难: 1. 没有理解dp数组及下标的含义 2. 推论公式 没有想到是 dp[i] = Math.min(dp[i-1] + cost[i-1], dp[i-2] + cost[i-2]) 太妙了

看完代码随想录之后的想法:

今日收获：

重点：
