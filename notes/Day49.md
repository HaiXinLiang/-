第九章 动态规划part10

● 121. 买卖股票的最佳时机 
● 122.买卖股票的最佳时机II 

 详细布置 

股票问题是一个动态规划的系列问题，今日安排的题目不多，大家可以慢慢消化。

 121. 买卖股票的最佳时机 
视频讲解：https://www.bilibili.com/video/BV1Xe4y1u77q

https://programmercarl.com/0121.%E4%B9%B0%E5%8D%96%E8%82%A1%E7%A5%A8%E7%9A%84%E6%9C%80%E4%BD%B3%E6%97%B6%E6%9C%BA.html

题目：https://leetcode.com/problems/best-time-to-buy-and-sell-stock

看到题目的第一想法：没想过递推公式可以由两个组成
           dp[i][0] = Math.max(dp[i-1][0], **-prices[i]**);  //第i天持有，可以是i-1天已经持有，或当天买入。因为整个过程只买卖一次所以是0-prices[i];
           dp[i][1] = Math.max(dp[i-1][1], dp[i-1][0] + prices[i]); //第i天不持有，可以是i-1天还没有持有，或当天买卖出

实现过程中遇到哪些困难: //dp[i][0] 持有股票最大现金， dp[i][1]不持有股票最大现金

看完代码随想录之后的想法:

今日收获：

重点：

 122.买卖股票的最佳时机II  
视频讲解：https://www.bilibili.com/video/BV1D24y1Q7Ls

https://programmercarl.com/0122.%E4%B9%B0%E5%8D%96%E8%82%A1%E7%A5%A8%E7%9A%84%E6%9C%80%E4%BD%B3%E6%97%B6%E6%9C%BAII%EF%BC%88%E5%8A%A8%E6%80%81%E8%A7%84%E5%88%92%EF%BC%89.html  

题目：https://leetcode.com/problems/best-time-to-buy-and-sell-stock-ii

看到题目的第一想法：没有想到过递推公式  有两个组成
            dp[i][0] = Math.max(dp[i-1][0], dp[i-1][1] - prices[i]); //第i天持有，可以是i-1天已经持有，或当天买入。当天买入时，可能已有利润dp[i-1][1]
            dp[i][1] = Math.max(dp[i-1][1], dp[i-1][0] + prices[i]);

实现过程中遇到哪些困难: //dp[i][0] 持有股票最大现金， dp[i][1]不持有股票最大现金

看完代码随想录之后的想法:

今日收获：

重点：
