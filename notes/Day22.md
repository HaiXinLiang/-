第六章 二叉树part08
今日内容： 

● 235. 二叉搜索树的最近公共祖先 

● 701.二叉搜索树中的插入操作 

● 450.删除二叉搜索树中的节点 


 详细布置 

 235. 二叉搜索树的最近公共祖先 

相对于 二叉树的最近公共祖先 本题就简单一些了，因为 可以利用二叉搜索树的特性。 

题目链接/文章讲解：https://programmercarl.com/0235.%E4%BA%8C%E5%8F%89%E6%90%9C%E7%B4%A2%E6%A0%91%E7%9A%84%E6%9C%80%E8%BF%91%E5%85%AC%E5%85%B1%E7%A5%96%E5%85%88.html

视频讲解：https://www.bilibili.com/video/BV1Zt4y1F7ww  

题目：https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-search-tree

看到题目的第一想法：有点很复杂的感觉，不知道是否要分别判断p, 和 q

实现过程中遇到哪些困难: 

看完代码随想录之后的想法: 看完视频后，感觉解题思路太秒了。二叉搜索树的公共祖先一定在p和q中间。所以不用单独判断p和q。

今日收获：

重点：

 701.二叉搜索树中的插入操作  

本题比想象中的简单，大家可以先自己想一想应该怎么做，然后看视频讲解，就发现 本题为什么比较简单了。

题目链接/文章讲解：https://programmercarl.com/0701.%E4%BA%8C%E5%8F%89%E6%90%9C%E7%B4%A2%E6%A0%91%E4%B8%AD%E7%9A%84%E6%8F%92%E5%85%A5%E6%93%8D%E4%BD%9C.html 

视频讲解：https://www.bilibili.com/video/BV1Et4y1c78Y  

题目：https://leetcode.com/problems/insert-into-a-binary-search-tree

看到题目的第一想法：看起来很复杂

实现过程中遇到哪些困难: 

看完代码随想录之后的想法:看过视频后实现很容易~

今日收获：

重点：

 450.删除二叉搜索树中的节点  

相对于 插入操作，本题就有难度了，涉及到改树的结构 

题目链接/文章讲解：https://programmercarl.com/0450.%E5%88%A0%E9%99%A4%E4%BA%8C%E5%8F%89%E6%90%9C%E7%B4%A2%E6%A0%91%E4%B8%AD%E7%9A%84%E8%8A%82%E7%82%B9.html  

视频讲解：https://www.bilibili.com/video/BV1tP41177us  

题目：https://leetcode.com/problems/delete-node-in-a-bst

看到题目的第一想法：

实现过程中遇到哪些困难: 返回的时候没有想到上一层递归是怎么接回去，看着参考代码答案+看第二次视频才有感悟。

if(root.val > key) **root.left =** deleteNode(root.left, key);

if(root.val < key) **root.right =** deleteNode(root.right, key);

看完代码随想录之后的想法:

今日收获：

重点：
