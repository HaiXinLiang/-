第九章 动态规划part03

● 343. 整数拆分 

● 96.不同的二叉搜索树 

 详细布置 

今天两题都挺有难度，建议大家思考一下没思路，直接看题解，第一次做，硬想很难想出来。

 343. 整数拆分 

https://programmercarl.com/0343.%E6%95%B4%E6%95%B0%E6%8B%86%E5%88%86.html   

视频讲解：https://www.bilibili.com/video/BV1Mg411q7YJ

题目：https://leetcode.com/problems/integer-break

看到题目的第一想法：直接看视频

实现过程中遇到哪些困难: 看完视频还是不太懂得那个递推公式是怎么来的。

看完代码随想录之后的想法: 对Karl给出的递推公式还是不怎么理解。在网上找到另外一个递推公式比较好理解。
// dp[i] = Math.max(dp[i], Math.max(j*(i-j), j*dp[i-j])); -- 不是太理解
   dp[i] = Math.max(dp[i], Math.max(j, dp[j]) * Math.max(i-j, dp[i-j])); -- 指j/i-j可以拆，也可以保持不变。
            

今日收获：写递推公式的时候，都需要对自己发出灵魂的拷问，问一问 dp数组的含义及下标的具体意思。

重点：dp[i] 是对i拆分，得到最大值dp[i]

 96.不同的二叉搜索树 

https://programmercarl.com/0096.%E4%B8%8D%E5%90%8C%E7%9A%84%E4%BA%8C%E5%8F%89%E6%90%9C%E7%B4%A2%E6%A0%91.html   

视屏讲解：https://www.bilibili.com/video/BV1eK411o7QA 

题目：https://leetcode.com/problems/unique-binary-search-trees

看到题目的第一想法：看完视频应该可以自己做处理。

实现过程中遇到哪些困难: 写递推公式的时候有点困难，得不断地问自己dp数组的含义及下标具体意义。一开始忘了是左右子树相乘，然后相加。后来慢慢想起Karl是如何推导递推公式的，加上debug，慢慢写出递推公式了。

看完代码随想录之后的想法:

今日收获：写递推公式的时候，都需要对自己发出灵魂的拷问，问一问 dp数组的含义及下标的具体意思。

重点：左右子树**相乘**，然后相加
