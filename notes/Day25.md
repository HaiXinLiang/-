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

题目：https://leetcode.com/problems/letter-combinations-of-a-phone-number

看到题目的第一想法：感觉不会做，虽然看了视频。强迫自己去做，开始打算定义不同数组代表不同的数字输入。偷看了参考答案，发现自己想多了，可以用一个数组就可以映射整个电话数字盘。

实现过程中遇到哪些困难: 偷看了数字盘可以用一个数组映射后，继续强迫自己做下去，按照回溯的temple写了下来。测试结果跟最终结果相差不远，只是多了一些由第二个数字的自我组合。然后没有看答案，自己想出来是因为用了两重for loop循环。

<img width="521" alt="image" src="https://user-images.githubusercontent.com/87255377/227824313-a6b15bb9-2263-4ce9-b3ad-72ed82abfd12.png">

<img width="364" alt="image" src="https://user-images.githubusercontent.com/87255377/227824693-e1d4e709-a25b-45cd-9254-f7ca74ae5337.png">


看完代码随想录之后的想法:

今日收获：


重点：
