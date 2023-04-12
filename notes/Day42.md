第九章 动态规划part04

● 01背包问题，你该了解这些！ 

● 01背包问题，你该了解这些！ 滚动数组  

● 416. 分割等和子集 

正式开始背包问题，背包问题还是挺难的，虽然大家可能看了很多背包问题模板代码，感觉挺简单，但基本理解的都不够深入。 

如果是直接从来没听过背包问题，可以先看文字讲解慢慢了解 这是干什么的。

如果做过背包类问题，可以先看视频，很多内容，是自己平时没有考虑到位的。 

背包问题，力扣上没有原题，大家先了解理论，今天就安排一道具体题目。 

 详细布置 

 01背包问题 二维 
https://programmercarl.com/%E8%83%8C%E5%8C%85%E7%90%86%E8%AE%BA%E5%9F%BA%E7%A1%8001%E8%83%8C%E5%8C%85-1.html  

视频讲解：https://www.bilibili.com/video/BV1cg411g7Y6  

数组含义： dp[i][j]: 表示从下标为【0-i】的物品里任意取，放进容量为j的背包，价值总和最大是多少。

![image](https://user-images.githubusercontent.com/87255377/231454818-bb91e114-2202-4cdf-8b4a-c47e52de8103.png)

递推公式： dp[i][j] = Math.max(dp[i-1][j], dp[i-1][j-weight[i]] + value[i]);

**不放物品i**：由dp[i - 1][j]推出，即背包容量为j，里面不放物品i的最大价值，此时dp[i][j]就是dp[i - 1][j]。(其实就是当物品i的重量大于背包j的重量时，物品i无法放进背包中，所以被背包内的价值依然和前面相同。)
**放物品i**：由dp[i - 1][j - weight[i]]推出，dp[i - 1][j - weight[i]] 为背包容量为j - weight[i]的时候不放物品i的最大价值，那么dp[i - 1][j - weight[i]] + value[i] （物品i的价值），就是背包放物品i得到的最大价值

初始化：
![image](https://user-images.githubusercontent.com/87255377/231455062-b5855e37-ba2d-4652-972f-d3ec092217a1.png)

遍历顺序：
for(int i =1; i<weight.length;i++){
  for(int j=1;j<=bageSize;j++){
     if(j<weight[i]){
       dp[i][j] = dp[i-1][j]; //当前背包容量小于物品i重量，放不下物品i
     }else{
       dp[i][j] = Math.max(dp[i-1][j], dp[i-1][j-weight[i]] + value[i]);
     }
   }
 }

 01背包问题 一维 
https://programmercarl.com/%E8%83%8C%E5%8C%85%E7%90%86%E8%AE%BA%E5%9F%BA%E7%A1%8001%E8%83%8C%E5%8C%85-2.html  

视频讲解：https://www.bilibili.com/video/BV1BU4y177kY  

dp[j]

dp[j] = Math.max(dp[j], dp[j-weight[i]] + value[i]



 416. 分割等和子集  
本题是 01背包的应用类题目
https://programmercarl.com/0416.%E5%88%86%E5%89%B2%E7%AD%89%E5%92%8C%E5%AD%90%E9%9B%86.html    

视频讲解：https://www.bilibili.com/video/BV1rt4y1N7jE

题目：https://leetcode.com/problems/partition-equal-subset-sum/

看到题目的第一想法：自己想试着做出来，但是没有想明白如何用dp做。

实现过程中遇到哪些困难: 后序遍历中 虽然知道是倒序遍历，但是忘了j的条件。 int[] dp = new int[**target + 1**]; 还没想清楚为什么

看完代码随想录之后的想法: 加深了对01背包问题的解法。

今日收获：这题 nums[i]即是重量也是value

重点：
