day 14 第六章二叉树
 今日内容： 
 

● 理论基础

● 递归遍历  

● 迭代遍历

● 统一迭代


 详细布置 

 理论基础  
 
 https://www.bilibili.com/video/BV1Hy4y1t7ij/

需要了解 二叉树的种类，存储方式，遍历方式 以及二叉树的定义 

/**
 * Definition for a binary tree node.
 * public class TreeNode {
 *     int val;
 *     TreeNode left;
 *     TreeNode right;
 *     TreeNode() {}
 *     TreeNode(int val) { this.val = val; }
 *     TreeNode(int val, TreeNode left, TreeNode right) {
 *         this.val = val;
 *         this.left = left;
 *         this.right = right;
 *     }
 * }
 */

文章讲解：https://programmercarl.com/%E4%BA%8C%E5%8F%89%E6%A0%91%E7%90%86%E8%AE%BA%E5%9F%BA%E7%A1%80.html  


递归遍历 （必须掌握） **递归三要素：1.确定递归函数的参数和返回值（一般是void）2.确定终止条件 3.去顶单层递归逻辑**

二叉树的三种递归遍历掌握其规律后，其实很简单 

题目链接/文章讲解/视频讲解：https://programmercarl.com/%E4%BA%8C%E5%8F%89%E6%A0%91%E7%9A%84%E9%80%92%E5%BD%92%E9%81%8D%E5%8E%86.html  

视频讲解： https://www.bilibili.com/video/BV1Wh411S7xt

题目：
https://leetcode.com/problems/binary-tree-preorder-traversal  //前序遍历：中左右
https://leetcode.com/problems/binary-tree-inorder-traversal  //中序遍历：左中右
https://leetcode.com/problems/binary-tree-postorder-traversal  //后序遍历：左右中

看到题目的第一想法： 

实现过程中遇到哪些困难: 看视频开头，觉得怎么三题这么多，后来明白，只要明白一题，其他的都很好写。

看完代码随想录之后的想法: 

今日收获：对二叉树有所了解，特别是其定义，有特别留意leecode上给出的代码。

重点： 递归三要素



迭代遍历 （基础不好的录友，迭代法可以放过）

题目链接/文章讲解/视频讲解：https://programmercarl.com/%E4%BA%8C%E5%8F%89%E6%A0%91%E7%9A%84%E8%BF%AD%E4%BB%A3%E9%81%8D%E5%8E%86.html  

 

统一迭代   （基础不好的录友，迭代法可以放过）

这是统一迭代法的写法， 如果学有余力，可以掌握一下

题目链接/文章讲解：https://programmercarl.com/%E4%BA%8C%E5%8F%89%E6%A0%91%E7%9A%84%E7%BB%9F%E4%B8%80%E8%BF%AD%E4%BB%A3%E6%B3%95.html  


往日任务
● day 1 任务以及具体安排：https://docs.qq.com/doc/DUG9UR2ZUc3BjRUdY 

● day 2 任务以及具体安排：https://docs.qq.com/doc/DUGRwWXNOVEpyaVpG 

● day 3 任务以及具体安排：https://docs.qq.com/doc/DUGdqYWNYeGhlaVR6 

● day 4 任务以及具体安排：https://docs.qq.com/doc/DUFNjYUxYRHRVWklp 

● day 5 周日休息

● day 6 任务以及具体安排：https://docs.qq.com/doc/DUEtFSGdreWRuR2p4

● day 7 任务以及具体安排：https://docs.qq.com/doc/DUElCb1NyTVpXa0Jj 

● day 8 任务以及具体安排：https://docs.qq.com/doc/DUGdsY2JFaFhDRVZH 

● day 9 任务以及具体安排：https://docs.qq.com/doc/DUHVXSnZNaXpVUHN4 


● day 10 任务以及具体安排：https://docs.qq.com/doc/DUElqeHh3cndDbW1Q 

●day 11 任务以及具体安排：https://docs.qq.com/doc/DUHh6UE5hUUZOZUd0 

●day 12 周日休息 

●day 13 任务以及具体安排：https://docs.qq.com/doc/DUHNpa3F4b2dMUWJ3 

