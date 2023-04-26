第九章 动态规划part16

● 583. 两个字符串的删除操作 
● 72. 编辑距离 
● 编辑距离总结篇   

 详细布置 

 583. 两个字符串的删除操作 

本题和动态规划：115.不同的子序列 相比，其实就是两个字符串都可以删除了，情况虽说复杂一些，但整体思路是不变的。
https://programmercarl.com/0583.%E4%B8%A4%E4%B8%AA%E5%AD%97%E7%AC%A6%E4%B8%B2%E7%9A%84%E5%88%A0%E9%99%A4%E6%93%8D%E4%BD%9C.html

视频：https://www.bilibili.com/video/BV1we4y157wB

题目：https://leetcode.com/problems/delete-operation-for-two-strings

看到题目的第一想法：看视频

实现过程中遇到哪些困难: 
解法一： 开始的时候对dp数组的定义不是太理解 //dp[i][j] : 以i-1结尾的word1, 以j-1结尾的word2，删除最少次数变成相同word
解法一的初始值定义 (开始的时候没有想明白）：  
 for(int i=0;i<=word1.length();i++){
            dp[i][0] = i;
        }

        for(int j=0;j<=word2.length();j++){
            dp[0][j] = j;
        }

解法二： dp数组定义：以i-1结尾的word1, 以j-1结尾的word2，最长相同子序列的长度 (不一定要连续的)

看完代码随想录之后的想法: 
今日收获：没有把最长相同子序列忘记， 呵呵

重点：

 72. 编辑距离 

最终我们迎来了编辑距离这道题目，之前安排题目都是为了 编辑距离做铺垫。 

https://programmercarl.com/0072.%E7%BC%96%E8%BE%91%E8%B7%9D%E7%A6%BB.html

视频：https://www.bilibili.com/video/BV1qv4y1q78f

题目：https://leetcode.com/problems/edit-distance

看到题目的第一想法：听说是最难的，直接看视频了

实现过程中遇到哪些困难: 
一，递推公式：  1. if(word1.charAt(i-1) == word2.charAt(j-1)) dp[i][j] = dp[i-1][j-1]; 
               2. else dp[i][j] = Math.min(
                                增/删  dp[i-1][j]+1 / dp[i][j-1]+1
                                替换   dp[i-1][j-1]+1)

看完代码随想录之后的想法: 要看代码随想录才知道 原来增删是同一递推公式

今日收获：

重点：

 编辑距离总结篇 
做一个总结吧
https://programmercarl.com/%E4%B8%BA%E4%BA%86%E7%BB%9D%E6%9D%80%E7%BC%96%E8%BE%91%E8%B7%9D%E7%A6%BB%EF%BC%8C%E5%8D%A1%E5%B0%94%E5%81%9A%E4%BA%86%E4%B8%89%E6%AD%A5%E9%93%BA%E5%9E%AB.html  

