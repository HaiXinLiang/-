day 11 第五章 栈与队列
今日内容： 

● 20. 有效的括号

● 1047. 删除字符串中的所有相邻重复项

● 150. 逆波兰表达式求值


 详细布置 

 20. 有效的括号 

讲完了栈实现队列，队列实现栈，接下来就是栈的经典应用了。 

大家先自己思考一下 有哪些不匹配的场景，在看视频 我讲的都有哪些场景，落实到代码其实就容易很多了。

题目链接/文章讲解/视频讲解：https://programmercarl.com/0020.%E6%9C%89%E6%95%88%E7%9A%84%E6%8B%AC%E5%8F%B7.html 

视频讲解：https://www.bilibili.com/video/BV1AF411w78g

题目：https://leetcode.com/problems/valid-parentheses

看到题目的第一想法： 想到有什么情况是无效的，因为例子中没有{【】}这样的例子。最后还是看了视频。发现karl总结得很到位，就是三种情况。

实现过程中遇到哪些困难:实现过程很顺利。但是写的code比较臃肿。

看完代码随想录之后的想法: 看了代码之后，知道如何改进了。

今日收获：改进代码，把需要pop的写在最后。

重点：栈的运用


 1047. 删除字符串中的所有相邻重复项 

栈的经典应用。 

要知道栈为什么适合做这种类似于爱消除的操作，因为栈帮助我们记录了 遍历数组当前元素时候，前一个元素是什么。

题目链接/文章讲解/视频讲解：https://programmercarl.com/1047.%E5%88%A0%E9%99%A4%E5%AD%97%E7%AC%A6%E4%B8%B2%E4%B8%AD%E7%9A%84%E6%89%80%E6%9C%89%E7%9B%B8%E9%82%BB%E9%87%8D%E5%A4%8D%E9%A1%B9.html  

视频讲解：https://www.bilibili.com/video/BV12a411P7mw

题目：https://leetcode.com/problems/remove-all-adjacent-duplicates-in-string

看到题目的第一想法： 跟前一题好像差不多，但是不敢肯定自己的想法，最后看了视频前2分钟才确认。

实现过程中遇到哪些困难:不知道怎样倒序回来。

看完代码随想录之后的想法: 真的如果这一题不是出现在stack与queue中的练习题，加上刚做了与它类似的上一题，有点难想象在这里用栈。

今日收获：尝试用deque去解题，而且了解一下[deque与stack的区别](https://www.baeldung.com/java-deque-vs-stack)，没有深入理解与自我总结=P

重点：重点竟然是deque里面的character如何换成string，而且要倒序~


150. 逆波兰表达式求值 

本题不难，但第一次做的话，会很难想到，所以先看视频，了解思路再去做题 

题目链接/文章讲解/视频讲解：https://programmercarl.com/0150.%E9%80%86%E6%B3%A2%E5%85%B0%E8%A1%A8%E8%BE%BE%E5%BC%8F%E6%B1%82%E5%80%BC.html  

视频讲解：https://www.bilibili.com/video/BV1kd4y1o7on

题目：https://leetcode.com/problems/evaluate-reverse-polish-notation

看到题目的第一想法： 还是看视频吧。

实现过程中遇到哪些困难:看了视频后自己做出来了。一开始没搞清楚‘+’与“+”的区别，debug的时候才发现出问题了。

看完代码随想录之后的想法: 自己的写法把检验是否是数字， 还有是否是有效的操作符也做了检验。

今日收获：‘+’与“+”的不同。

重点：


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

