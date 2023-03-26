第七章 回溯算法part02


今日内容： 

● 216.组合总和III

● 17.电话号码的字母组合


 详细布置 

 216.组合总和III 

如果把 组合问题理解了，本题就容易一些了。 

题目链接/文章讲解：https://programmercarl.com/0216.%E7%BB%84%E5%90%88%E6%80%BB%E5%92%8CIII.html   

视频讲解：https://www.bilibili.com/video/BV1wg411873x

题目：https://leetcode.com/problems/combination-sum-iii

看到题目的第一想法：

实现过程中遇到哪些困难: 1. 没有把path的元素在适当的位置加上，应该在for循环里面加的，但在叶子（收获结果）那里处理。 2. 把startIndex作为元素加入path里面的，应该是加变化的i。
3. 不可以放i++,  或k--进去backtracking函数里面，只能是i+1, k-1.

看完代码随想录之后的想法: 还没有很好的掌握回溯。

今日收获：

重点：


 17.电话号码的字母组合 

本题大家刚开始做会有点难度，先自己思考20min，没思路就直接看题解。 

题目链接/文章讲解：https://programmercarl.com/0017.%E7%94%B5%E8%AF%9D%E5%8F%B7%E7%A0%81%E7%9A%84%E5%AD%97%E6%AF%8D%E7%BB%84%E5%90%88.html   

视频讲解：https://www.bilibili.com/video/BV1yV4y1V7Ug
