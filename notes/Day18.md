第六章 二叉树 part05
  今日内容 

● 513.找树左下角的值

● 112. 路径总和  113.路径总和ii

● 106.从中序与后序遍历序列构造二叉树 105.从前序与中序遍历序列构造二叉树


 详细布置 

 找树左下角的值  

本地递归偏难，反而迭代简单属于模板题， 两种方法掌握一下 

题目链接/文章讲解/视频讲解：https://programmercarl.com/0513.%E6%89%BE%E6%A0%91%E5%B7%A6%E4%B8%8B%E8%A7%92%E7%9A%84%E5%80%BC.html  

 路径总和  

本题 又一次设计要回溯的过程，而且回溯的过程隐藏的还挺深，建议先看视频来理解

视频讲解: https://www.bilibili.com/video/BV1424y1Z7pn

题目：https://leetcode.com/problems/find-bottom-left-tree-value

看到题目的第一想法： 看了视频后做的，但是也是有点乱。得重新看了视频后再写出来。

实现过程中遇到哪些困难:没有把result和maxDepth的定义放在最外面。

看完代码随想录之后的想法: 

今日收获：中央variable， result 与 maxDepth

重点：中， 不处理。 只要左在右前面就行。所以前中后序遍历都可以。

112. 路径总和，和 113. 路径总和ii 一起做了。 优先掌握递归法。

题目链接/文章讲解/视频讲解：https://programmercarl.com/0112.%E8%B7%AF%E5%BE%84%E6%80%BB%E5%92%8C.html  

 从中序与后序遍历序列构造二叉树 

本题算是比较难的二叉树题目了，大家先看视频来理解。 

视频讲解: https://www.bilibili.com/video/BV19t4y1L7CR

题目：https://leetcode.com/problems/path-sum-ii

看到题目的第一想法： 

实现过程中遇到哪些困难:
  112题 - 找到后，要记得向上传递！if(left) return true; if(right) return true; 
  113题.pathList和pathNodes都是参数，因为递归函数里面要更改。（开始的时候没有加入递归函数里面）。 找到符合pathNodes， 要new ArrayList<>()放入pathList。不然pathNodes地址所放的值再后面会改变的。

看完代码随想录之后的想法: 

今日收获：再次加深什么参数需要放在函数里面。 

重点：递归完要回溯。pathList.add(**new ArrayList<>(pathNodes)**);

106.从中序与后序遍历序列构造二叉树，105.从前序与中序遍历序列构造二叉树 一起做，思路一样的

题目链接/文章讲解/视频讲解：https://programmercarl.com/0106.%E4%BB%8E%E4%B8%AD%E5%BA%8F%E4%B8%8E%E5%90%8E%E5%BA%8F%E9%81%8D%E5%8E%86%E5%BA%8F%E5%88%97%E6%9E%84%E9%80%A0%E4%BA%8C%E5%8F%89%E6%A0%91.html

视频讲解: https://www.bilibili.com/video/BV1vW4y1i7dn

题目：

看到题目的第一想法： 

实现过程中遇到哪些困难:切割的原理是搞明白了，但是对postorder代码的分割点，有点疑惑，不是太理解。。。
int lenOfLeft = rootIndex - inBegin;

root.left = findNode(inorder, inBegin, rootIndex, postorder, postBegin, **postBegin + lenOfLeft**);  有空后期要debug一下。

看完代码随想录之后的想法: 

今日收获

重点：
