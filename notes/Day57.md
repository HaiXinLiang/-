第九章 动态规划part17

● 647. 回文子串  

● 516.最长回文子序列

● 动态规划总结篇

今天 我们就要结束动态规划章节了，大家激不激动！！！ 

 详细布置 

 647. 回文子串   

动态规划解决的经典题目，如果没接触过的话，别硬想 直接看题解。
https://programmercarl.com/0647.%E5%9B%9E%E6%96%87%E5%AD%90%E4%B8%B2.html  

视频：https://www.bilibili.com/video/BV17G4y1y7z9

题目：https://leetcode.com/problems/palindromic-substrings

看到题目的第一想法：

实现过程中遇到哪些困难: 1.数组的定义： dp[i][j]： 表示区间范围[i,j] （注意是左闭右闭）的子串是否是回文子串 
                      2.递推公式：if((**j-i<=1**) || (dp[i+1][j-1])){  //还没有搞清楚为什么要<=1, 而只判断i==j是不行的
                        dp[i][j] = true;
                        res++;
                    }
                    
                    3. 遍历顺利与以前的很不一样

看完代码随想录之后的想法: 

今日收获：

重点：

 516.最长回文子序列 
 
 647. 回文子串，求的是回文子串，而本题要求的是回文子序列， 大家要搞清楚两者之间的区别。 
https://programmercarl.com/0516.%E6%9C%80%E9%95%BF%E5%9B%9E%E6%96%87%E5%AD%90%E5%BA%8F%E5%88%97.html  

视频：https://www.bilibili.com/video/BV1d8411K7W6

题目：https://leetcode.com/problems/longest-palindromic-subsequence

看到题目的第一想法：

实现过程中遇到哪些困难: 1. 数组的定义  //dp[i][j] 表示[i,j]最长的回文子串长度  
                      2. 递推公式  
                      if(s.charAt(i) == s.charAt(j)){
                    dp[i][j] = dp[i+1][j-1] + **2**;  // 刚开始是写了+1，忘了是应该+2，
                }else{
                    dp[i][j] = Math.max(dp[i+1][j], dp[i][j-1]);
                }
                 3. 初始化
                 for(int i=0;i<s.length();i++){
                  dp[i][i] = 1;
                 }

看完代码随想录之后的想法:

今日收获：

重点：

 动态规划总结篇 
https://programmercarl.com/%E5%8A%A8%E6%80%81%E8%A7%84%E5%88%92%E6%80%BB%E7%BB%93%E7%AF%87.html  
