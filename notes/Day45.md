第九章 动态规划part07

● 70. 爬楼梯 （进阶）

● 322. 零钱兑换 

● 279.完全平方数 

 详细布置 

 70. 爬楼梯 （进阶） 

这道题目 爬楼梯之前我们做过，这次再用完全背包的思路来分析一遍 

https://programmercarl.com/0070.%E7%88%AC%E6%A5%BC%E6%A2%AF%E5%AE%8C%E5%85%A8%E8%83%8C%E5%8C%85%E7%89%88%E6%9C%AC.html  

题目：https://leetcode.com/problems/climbing-stairs/

看到题目的第一想法：转换为完全背包问题来考虑，用int[] steps = {1,2}装着，然后是排列数问题， 先遍历背包 （target），再遍历物品 （步数）。

实现过程中遇到哪些困难: 

看完代码随想录之后的想法:

今日收获：用另外一个角度，解决同一个问题

重点：

 322. 零钱兑换  

如果求组合数就是外层for循环遍历物品，内层for遍历背包。
如果求排列数就是外层for遍历背包，内层for循环遍历物品。

这句话结合本题 大家要好好理解。
视频讲解：https://www.bilibili.com/video/BV14K411R7yv
https://programmercarl.com/0322.%E9%9B%B6%E9%92%B1%E5%85%91%E6%8D%A2.html  

题目：https://leetcode.com/problems/coin-change

看到题目的第一想法：自己试做，想到了dp[j]的定义，递推公式写对了(yeah!!!)

实现过程中遇到哪些困难: 1. 只依照范例，把dp[0]初始化成为0，没有考虑到其他非0下标的初始值。因为一直都是0.但是这次根据递推公式，求的是min，所以其他非0下标初始值是Integer的最大值。
2.导致在递推公式也没有考虑到只有dp[j-coins[i]]不是初始最大值时，该位才有选择的必要

看完代码随想录之后的想法: 跟着carl学算法

今日收获：自己写出了递推公式

重点：

 279.完全平方数  
本题 和 322. 零钱兑换 基本是一样的，大家先自己尝试做一做 
视频讲解：https://www.bilibili.com/video/BV12P411T7Br

https://programmercarl.com/0279.%E5%AE%8C%E5%85%A8%E5%B9%B3%E6%96%B9%E6%95%B0.html  

题目：https://leetcode.com/problems/perfect-squares/

看到题目的第一想法：自己试做，没做出来

实现过程中遇到哪些困难: 1. 不知道物品的集合 2. 遍历物品条件没写好。 i*i<**=**n

看完代码随想录之后的想法:

for(int i=1;**i*i<=n**;i++){
            for(int j=i*i;j<=n;j++)
                if(dp[j-i*i] != max){
                    dp[j] = Math.min(dp[j], dp[j-i*i] + 1);
                }
        }

今日收获：动态物品集合。 还是有点朦胧。但对遍历条件进一步加深

重点：
