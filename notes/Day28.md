28 第七章 回溯算法

● 93.复原IP地址 

● 78.子集 

● 90.子集II  

 详细布置 

 93.复原IP地址  

本期本来是很有难度的，不过 大家做完 分割回文串 之后，本题就容易很多了 

题目链接/文章讲解：https://programmercarl.com/0093.%E5%A4%8D%E5%8E%9FIP%E5%9C%B0%E5%9D%80.html  

视频讲解：https://www.bilibili.com/video/BV1XP4y1U73i/

题目：https://leetcode.com/problems/restore-ip-addresses

看到题目的第一想法：自己尝试去做。做出来了！yeah. 不过效率不高

实现过程中遇到哪些困难: 问题出现在，自己不会用stringbuilder的delete function，没能数清楚如何回溯的位置。 还有没有很好地剪枝。

看完代码随想录之后的想法:

今日收获：

重点：

 78.子集  

子集问题，就是收集树形结构中，每一个节点的结果。 整体代码其实和 回溯模板都是差不多的。 

题目链接/文章讲解：https://programmercarl.com/0078.%E5%AD%90%E9%9B%86.html  

视频讲解：https://www.bilibili.com/video/BV1U84y1q7Ci 

题目：https://leetcode.com/problems/subsets

看到题目的第一想法：看到题目感觉很熟悉，好像跟之前相类似，但又说不清哪里不同。

实现过程中遇到哪些困难: 

看完代码随想录之后的想法: 看了视频后才明白过来，原来这题跟之前组合问题的不同是在于，子集的结果收集在每个节点上，而组合或之前做过的题目收获结果都在树枝上。

今日收获：认识如何在每个节点上收获结果，以及这跟在树枝上收获结果的区别。

重点：论画出树形图的重要性。要慢慢跟着学话树形机构！

90.子集II 

大家之前做了 40.组合总和II 和 78.子集 ，本题就是这两道题目的结合，建议自己独立做一做，本题涉及的知识，之前都讲过，没有新内容。 

题目链接/文章讲解：https://programmercarl.com/0090.%E5%AD%90%E9%9B%86II.html   

视频讲解：https://www.bilibili.com/video/BV1vm4y1F71J

题目：https://leetcode.com/problems/subsets-ii

看到题目的第一想法：应该可以自己做出来。

实现过程中遇到哪些困难: 做了99.99%了，就是差了一点点没运行过关。一开始不小心写了i>1，其实心里想着是应该>=1,从i=1开始判断）

<img width="388" alt="image" src="https://user-images.githubusercontent.com/87255377/228245525-1b94b418-70a8-44bd-94e0-ba449ace64b8.png">


看完代码随想录之后的想法:看了文字答案后才发现问题所在

今日收获：重新复习了树层去重。

重点：
