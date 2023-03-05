4 第二章 链表

● day 1 任务以及具体安排：https://docs.qq.com/doc/DUG9UR2ZUc3BjRUdY 

● day 2 任务以及具体安排：https://docs.qq.com/doc/DUGRwWXNOVEpyaVpG 

● day 3 任务以及具体安排：https://docs.qq.com/doc/DUGdqYWNYeGhlaVR6

 
今日任务 

● 24. 两两交换链表中的节点 

● 19.删除链表的倒数第N个节点

● 面试题 02.07. 链表相交 

● 142.环形链表II 

● 总结

 详细布置 

 24. 两两交换链表中的节点 

用虚拟头结点，这样会方便很多。 

本题链表操作就比较复杂了，建议大家先看视频，视频里我讲解了注意事项，为什么需要temp保存临时节点。

题目链接/文章讲解/视频讲解： https://programmercarl.com/0024.%E4%B8%A4%E4%B8%A4%E4%BA%A4%E6%8D%A2%E9%93%BE%E8%A1%A8%E4%B8%AD%E7%9A%84%E8%8A%82%E7%82%B9.html

视频讲解： https://www.bilibili.com/video/BV1YT411g7br

题目：https://leetcode.com/problems/swap-nodes-in-pairs/

看到题目的第一想法：以为自己链表的知识有一定认识，应该可以拿下。结果没有拿下，要看视频后，才实现下来。

实现过程中遇到哪些困难: 今天没有看视频先做的，做了很久都没有做出来。一看视频知道自己错在哪里了。

看完代码随想录之后的想法:讲得很清晰。只写了统一操作的那种方法。

今日收获：加入了虚拟头节点，但运用得不好。

重点：1. cur应该放在变化的节点前 2. 交换也没有交换彻底，没想到要添加两个temp的值，只想到了添加一个（汗颜）

 19.删除链表的倒数第N个节点  

双指针的操作，要注意，删除第N个节点，那么我们当前遍历的指针一定要指向 第N个节点的前一个节点，建议先看视频。

题目链接/文章讲解/视频讲解：https://programmercarl.com/0019.%E5%88%A0%E9%99%A4%E9%93%BE%E8%A1%A8%E7%9A%84%E5%80%92%E6%95%B0%E7%AC%ACN%E4%B8%AA%E8%8A%82%E7%82%B9.html

视频讲解： https://www.bilibili.com/video/BV1vW4y1U7Gf

题目：https://leetcode.com/problems/remove-nth-node-from-end-of-list/

看到题目的第一想法：不知道怎么找到N。

实现过程中遇到哪些困难: 如何找N，临界值while的判断

看完代码随想录之后的想法:看了视频后，觉得用双指针找倒数第N/N+1个，太绝妙了。

今日收获：1. 宗旨，要在改动链接节点前做指针标志 2. 双指针找倒数第N/N+1个节点

重点：双指针，哪里做指针
 

160. 面试题 02.07. 链表相交  

本题没有视频讲解，大家注意 数值相同，不代表指针相同。

题目链接/文章讲解：https://programmercarl.com/%E9%9D%A2%E8%AF%95%E9%A2%9802.07.%E9%93%BE%E8%A1%A8%E7%9B%B8%E4%BA%A4.html

视频讲解： N/A

题目：https://leetcode.com/problems/intersection-of-two-linked-lists/

看到题目的第一想法：如果可以倒过来，先判断最后一个是否相等，然后不断向前就好了。看了文章讲解，才了解是先分别算两链表的长度，再从倒数相同位数那里对比两个列表。

实现过程中遇到哪些困难:看完文章讲解后，做起题目很顺利。

今日收获：感觉自己用指针，运用比前几道题灵活不少。

重点：intersection of two linked lists 的 intersection 是指相同的内存地址


 142.环形链表II  

算是链表比较有难度的题目，需要多花点时间理解 确定环和找环入口，建议先看视频。

题目链接/文章讲解/视频讲解：https://programmercarl.com/0142.%E7%8E%AF%E5%BD%A2%E9%93%BE%E8%A1%A8II.html

视频讲解： https://www.bilibili.com/video/BV1if4y1d7ob

题目：https://leetcode.com/problems/linked-list-cycle-ii/

看到题目的第一想法：只要next没有出现null, 就是有闭环了，但不知道怎么找到环的入口节点。

实现过程中遇到哪些困难: 数学逻辑得过关。明白了逻辑关系，就很容易实现了。

看完代码随想录之后的想法:看了视频后，觉得太绝妙了，得数学好，想通了才能很好把题攻克。

今日收获：1. 双指针找闭环，快慢指针能相遇，就是有闭环。 2. 快指针一定在慢指针走一圈内环的时候相遇，不可能跑到两圈才相遇。3.相遇后的点-》闭环入口节点 的长度等于 head节点到闭环入口节点的长度

重点：数学逻辑过关才能把题做出来
