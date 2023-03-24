第六章 二叉树part09

 今日内容：

● 669. 修剪二叉搜索树 

● 108.将有序数组转换为二叉搜索树 

● 538.把二叉搜索树转换为累加树 

● 总结篇 

 详细布置 

 669. 修剪二叉搜索树 

这道题目比较难，比 添加增加和删除节点难的多，建议先看视频理解。

题目链接/文章讲解： https://programmercarl.com/0669.%E4%BF%AE%E5%89%AA%E4%BA%8C%E5%8F%89%E6%90%9C%E7%B4%A2%E6%A0%91.html  

视频讲解： https://www.bilibili.com/video/BV17P41177ud  

题目：

看到题目的第一想法：

实现过程中遇到哪些困难: 

看完代码随想录之后的想法:

今日收获：如何接住递归返回值

重点：


 108.将有序数组转换为二叉搜索树  

本题就简单一些，可以尝试先自己做做。

https://programmercarl.com/0108.%E5%B0%86%E6%9C%89%E5%BA%8F%E6%95%B0%E7%BB%84%E8%BD%AC%E6%8D%A2%E4%B8%BA%E4%BA%8C%E5%8F%89%E6%90%9C%E7%B4%A2%E6%A0%91.html  

视频讲解：https://www.bilibili.com/video/BV1uR4y1X7qL  

题目：

看到题目的第一想法：

实现过程中遇到哪些困难: int index = **begin +** (end - begin)/2; 划分中节点的时候忘了把begin值加回去。

看完代码随想录之后的想法:

今日收获：

重点：**如何构造二叉树，整体思路，选取中间节点，将数组划分为左右区间，然后递归去遍历左右区间。**

 538.把二叉搜索树转换为累加树  

本题也不难，在 求二叉搜索树的最小绝对差 和 众数 那两道题目 都讲过了 双指针法，思路是一样的。

https://programmercarl.com/0538.%E6%8A%8A%E4%BA%8C%E5%8F%89%E6%90%9C%E7%B4%A2%E6%A0%91%E8%BD%AC%E6%8D%A2%E4%B8%BA%E7%B4%AF%E5%8A%A0%E6%A0%91.html 

视频讲解：https://www.bilibili.com/video/BV1d44y1f7wP

题目：https://leetcode.com/problems/convert-bst-to-greater-tree

看到题目的第一想法：

实现过程中遇到哪些困难: 刚开始的时候把sum作为参数传进入递归函数那，看了答案才知道不能这样子。要区分一下为什么！仔细想了一下，回归函数的参数是会回溯的。 就是会变回递归前。

看完代码随想录之后的想法:

今日收获：

重点：


 总结篇  

好了，二叉树大家就这样刷完了，做一个总结吧

https://programmercarl.com/%E4%BA%8C%E5%8F%89%E6%A0%91%E6%80%BB%E7%BB%93%E7%AF%87.html   
