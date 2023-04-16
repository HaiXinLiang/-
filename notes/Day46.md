第九章 动态规划part08

● 139.单词拆分 

● 关于多重背包，你该了解这些！ 

● 背包问题总结篇！  

 详细布置 

关于 多重背包，力扣上没有相关的题目，所以今天大家的重点就是回顾一波 自己做的背包题目吧。 

 139.单词拆分 
视频讲解：https://www.bilibili.com/video/BV1pd4y147Rh

https://programmercarl.com/0139.%E5%8D%95%E8%AF%8D%E6%8B%86%E5%88%86.html

题目：https://leetcode.com/problems/word-break

看到题目的第一想法：1.没想过可以用背包的解决思路。： 物品是wordDict， 然后去装满背包string， 而且是要排列循序装。妙妙妙  
2. 没有想到递推公式 是 if((j,i) 能在wordDict找到 && dp[j] is true) dp[i] is true 
3. 即使想到递推公式，也未必能能用code表达。
4. 遍历顺序及条件。排列顺序，先遍历背包，再遍历物品。


实现过程中遇到哪些困难: 

看完代码随想录之后的想法:

今日收获：太难了。

重点：

 关于多重背包，你该了解这些！ 

https://programmercarl.com/%E8%83%8C%E5%8C%85%E9%97%AE%E9%A2%98%E7%90%86%E8%AE%BA%E5%9F%BA%E7%A1%80%E5%A4%9A%E9%87%8D%E8%83%8C%E5%8C%85.html

 背包问题总结篇！ 

https://programmercarl.com/%E8%83%8C%E5%8C%85%E6%80%BB%E7%BB%93%E7%AF%87.html 
