第九章 动态规划 part05
● 1049. 最后一块石头的重量 II 
● 494. 目标和 
● 474.一和零  

 详细布置 

 1049. 最后一块石头的重量 II 

本题就和 昨天的 416. 分割等和子集 很像了，可以尝试先自己思考做一做。 

视频讲解：https://www.bilibili.com/video/BV14M411C7oV 

https://programmercarl.com/1049.%E6%9C%80%E5%90%8E%E4%B8%80%E5%9D%97%E7%9F%B3%E5%A4%B4%E7%9A%84%E9%87%8D%E9%87%8FII.html  

题目：https://leetcode.com/problems/last-stone-weight-ii/

看到题目的第一想法：开始想自己做，但是想了一下，还是没有头绪。

实现过程中遇到哪些困难: 看了视频，了解了解题思路，听着Karl的讲解，就自己开始着手做了。

看完代码随想录之后的想法:

今日收获：好像有点了解dp[target]的含义 在这题的含义，就是背包最大为target，实际上是接近target的值。

重点：

 494. 目标和 
大家重点理解 递推公式：dp[j] += dp[j - nums[i]]，这个公式后面的提问 我们还会用到。  

视频讲解：https://www.bilibili.com/video/BV1o8411j73x

https://programmercarl.com/0494.%E7%9B%AE%E6%A0%87%E5%92%8C.html  

题目：https://leetcode.com/problems/target-sum

看到题目的第一想法：看了视频再做

实现过程中遇到哪些困难: 遍历顺序物品是从0开始

dp[j] 容量为j 有dp[j]种方法。

已有物品1， dp[4] 凑成 dp[5]
已有物品2， dp[3] 凑成 dp[5]
已有物品3， dp[2] 凑成 dp[5]
已有物品4， dp[1] 凑成 dp[5]
已有物品5， dp[0] 凑成 dp[5]

看完代码随想录之后的想法: 深刻理解了，有多少种拿取的方法 dp[j] += dp[j-nums[i]]

今日收获：dp[j] += dp[j-nums[i]]

重点：dp[j] += dp[j-nums[i]]


 474.一和零  
通过这道题目，大家先粗略了解， 01背包，完全背包，多重背包的区别，不过不用细扣，因为后面 对于 完全背包，多重背包 还有单独讲解。

视频讲解：https://www.bilibili.com/video/BV1rW4y1x7ZQ 

https://programmercarl.com/0474.%E4%B8%80%E5%92%8C%E9%9B%B6.html  

题目：

看到题目的第一想法：

实现过程中遇到哪些困难: 

看完代码随想录之后的想法:

今日收获：

重点：
