第七章 回溯算法part03

● 39. 组合总和

● 40.组合总和II

● 131.分割回文串

 详细布置 

 39. 组合总和 

本题是 集合里元素可以用无数次，那么和组合问题的差别 其实仅在于 startIndex上的控制

题目链接/文章讲解：https://programmercarl.com/0039.%E7%BB%84%E5%90%88%E6%80%BB%E5%92%8C.html 

视频讲解：https://www.bilibili.com/video/BV1KT4y1M7HJ  

题目：https://leetcode.com/problems/combination-sum

看到题目的第一想法： 自己可以做出来。

实现过程中遇到哪些困难: 经常把backtracking函数里面那个i （下一层的startIndex），直接写startIndex。就是把上一层的startIndex传给了下一层的startIndex。这没有达到枝叶去重的效果。
<img width="309" alt="image" src="https://user-images.githubusercontent.com/87255377/227926240-90dd1840-0c76-4574-9457-0c2e20ee99cd.png">


看完代码随想录之后的想法:

今日收获：自己真的可以独立做出来

重点：

 40.组合总和II 

本题开始涉及到一个问题了：去重。

注意题目中给我们 集合是有重复元素的，那么求出来的 组合有可能重复，但题目要求不能有重复组合。 

题目链接/文章讲解：https://programmercarl.com/0040.%E7%BB%84%E5%90%88%E6%80%BB%E5%92%8CII.html   

视频讲解：https://www.bilibili.com/video/BV12V4y1V73A

题目：https://leetcode.com/problems/combination-sum-ii

看到题目的第一想法：自己试做了一下，发现没有去重。

实现过程中遇到哪些困难: 1. 不知道如何去重，也没有搞清楚**树层去重**和**树枝去重**的不同之处，2. 把上一层的startIndex直接传给了下一层做startIndex。 3. continue 与 return的区别是什么？？？ return是返回去原调用函数。continue是返回到for循环。

看完代码随想录之后的想法:好好想想如何做数层去重，是利用boolean[] used来标识

今日收获：知道了数层去重和树枝去重。

重点：

 131.分割回文串  

本题较难，大家先看视频来理解 分割问题，明天还会有一道分割问题，先打打基础。 

https://programmercarl.com/0131.%E5%88%86%E5%89%B2%E5%9B%9E%E6%96%87%E4%B8%B2.html  

视频讲解：https://www.bilibili.com/video/BV1c54y1e7k6  

题目：

看到题目的第一想法：

实现过程中遇到哪些困难: 

看完代码随想录之后的想法:

今日收获：

重点：
