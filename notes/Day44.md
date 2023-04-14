第九章 动态规划part06
● 完全背包
● 518. 零钱兑换 II 
● 377. 组合总和 Ⅳ  

  详细布置 

力扣上没有纯粹的完全背包的题目，所以大家看本篇了解一下 完全背包的理论 

后面的两道题目，都是完全背包的应用，做做感受一下 

 完全背包 
视频讲解：https://www.bilibili.com/video/BV1uK411o7c9

https://programmercarl.com/%E8%83%8C%E5%8C%85%E9%97%AE%E9%A2%98%E7%90%86%E8%AE%BA%E5%9F%BA%E7%A1%80%E5%AE%8C%E5%85%A8%E8%83%8C%E5%8C%85.html   

 518. 零钱兑换 II  

视频讲解：https://www.bilibili.com/video/BV1KM411k75j

https://programmercarl.com/0518.%E9%9B%B6%E9%92%B1%E5%85%91%E6%8D%A2II.html  

题目：https://leetcode.com/problems/coin-change-ii

看到题目的第一想法：自己试做一下，然后对照答案，发现dp数组的定义对了，遍历条件和循序也对了。就是递推公司错了。忘了这里求的是**多少种方法**

实现过程中遇到哪些困难: 求有多少种方法的递推公式是 dp[j] += dp[j-coins[i]];

看完代码随想录之后的想法:

今日收获：求有多少种方法，要确定是组合数，还是排列数。

组合法：先遍历物品，再遍历背包。
排列法：先遍历背包，再遍历物品。


 377. 组合总和 Ⅳ  
视频讲解：https://www.bilibili.com/video/BV1V14y1n7B6

https://programmercarl.com/0377.%E7%BB%84%E5%90%88%E6%80%BB%E5%92%8C%E2%85%A3.html

题目： https://leetcode.com/problems/combination-sum-iv

看到题目的第一想法：一开始以为这题与前一题一模一样。但是原来是不同的。上一题的题目是组合法，这题目是排列法。看完上题的视频才知道有区别。然后就做出来了。

实现过程中遇到哪些困难: 没有看好题目，没有看好是组合法，还是排列法

看完代码随想录之后的想法:

今日收获：求有多少种方法，要确定是组合数，还是排列数。

**组合法：先遍历物品，再遍历背包。
排列法：先遍历背包，再遍历物品。**

