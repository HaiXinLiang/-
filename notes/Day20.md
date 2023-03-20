第六章 二叉树 part06

今日内容 

● 654.最大二叉树 

● 617.合并二叉树 

● 700.二叉搜索树中的搜索 

● 98.验证二叉搜索树 



 详细布置 

654.最大二叉树 

又是构造二叉树，昨天大家刚刚做完 中序后序确定二叉树，今天做这个 应该会容易一些， 先看视频，好好体会一下 为什么构造二叉树都是 前序遍历 

题目链接/文章讲解：https://programmercarl.com/0654.%E6%9C%80%E5%A4%A7%E4%BA%8C%E5%8F%89%E6%A0%91.html  

视频讲解：https://www.bilibili.com/video/BV1MG411G7ox  

题目：https://leetcode.com/problems/maximum-binary-tree

看到题目的第一想法：

实现过程中遇到哪些困难: 按照昨天的解题思路，很快就做出来了。

看完代码随想录之后的想法: 跟昨天的思路很相似

今日收获：继续用map

重点：

 617.合并二叉树 

这次是一起操作两个二叉树了， 估计大家也没一起操作过两个二叉树，也不知道该如何一起操作，可以看视频先理解一下。 优先掌握递归。

题目链接/文章讲解：https://programmercarl.com/0617.%E5%90%88%E5%B9%B6%E4%BA%8C%E5%8F%89%E6%A0%91.html  

视频讲解：https://www.bilibili.com/video/BV1m14y1Y7JK  

题目：https://leetcode.com/problems/merge-two-binary-trees

看到题目的第一想法：

实现过程中遇到哪些困难: 

看完代码随想录之后的想法:看完视频写， 不难写。

今日收获：

重点：

 700.二叉搜索树中的搜索 

递归和迭代 都可以掌握以下，因为本题比较简单， 了解一下 二叉搜索树的特性

题目链接/文章讲解: https://programmercarl.com/0700.%E4%BA%8C%E5%8F%89%E6%90%9C%E7%B4%A2%E6%A0%91%E4%B8%AD%E7%9A%84%E6%90%9C%E7%B4%A2.html  

视频讲解：https://www.bilibili.com/video/BV1wG411g7sF   

题目：

看到题目的第一想法：自己做出来，用普通二叉树的方法。然后了解到二叉搜索树的特性

实现过程中遇到哪些困难: 

看完代码随想录之后的想法:

今日收获：二叉搜索树的特性。

重点：

 98.验证二叉搜索树 

遇到 搜索树，一定想着中序遍历，这样才能利用上特性。 

但本题是有陷阱的，可以自己先做一做，然后在看题解，看看自己是不是掉陷阱里了。这样理解的更深刻。

题目链接/文章讲解：https://programmercarl.com/0098.%E9%AA%8C%E8%AF%81%E4%BA%8C%E5%8F%89%E6%90%9C%E7%B4%A2%E6%A0%91.html 

视频讲解：https://www.bilibili.com/video/BV18P411n7Q4  

题目：https://leetcode.com/problems/validate-binary-search-tree/

看到题目的第一想法：真的需要用中序吗？我就用了后序，结果就打脸了。

实现过程中遇到哪些困难: 陷阱：误区：if(root.val > root.left && root.val < root.right) return true 这是错的。
例如
<img width="111" alt="image" src="https://user-images.githubusercontent.com/87255377/226340381-59456b48-9263-49cc-a5a3-3c0725015a8e.png">


看完代码随想录之后的想法:对于中间的处理不是很懂。

今日收获：搜索树，用中序遍历

重点：
