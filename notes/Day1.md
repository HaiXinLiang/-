数组理论基础，704. 二分查找，27. 移除元素

详细布置

数组理论基础
文章链接：https://programmercarl.com/%E6%95%B0%E7%BB%84%E7%90%86%E8%AE%BA%E5%9F%BA%E7%A1%80.html
题目建议： 了解一下数组基础，以及数组的内存空间地址，数组也没那么简单。


704. 二分查找
     题目建议： 大家能把 704 掌握就可以，35.搜索插入位置 和 34. 在排序数组中查找元素的第一个和最后一个位置 ，如果有时间就去看一下，没时间可以先不看，二刷的时候在看。
     先把 704写熟练，要熟悉 根据 左闭右开，左闭右闭 两种区间规则 写出来的二分法.
     
     题目链接：https://leetcode.cn/problems/binary-search
     
     文章讲解：https://programmercarl.com/0704.%E4%BA%8C%E5%88%86%E6%9F%A5%E6%89%BE.htm
     
     视频讲解：https://www.bilibili.com/video/BV1fA4y1o715
     
     题目：https://leetcode.com/problems/binary-search/
     
     看到题目的第一想法： 感觉好熟悉，自己一定会做，因为昨天已经看了相关视频
     
     实现过程中遇到哪些困难: 1. 排序和数值没区分好，2. 题目没看清楚，感觉无从下手，3. 最后还是得debug code 才能把其中的逻辑关系搞清楚
     
     看完代码随想录之后的想法: 每一句都有解释，条理很清晰。
     
     今日收获：1.题目得看清楚，数组是升排序的。 2. 排序和数值得区分运用，别混乱。3. 左闭右开，左闭右闭 昨天看了视频，今天做题，虽然感觉昨天好像懂了，其实下手做，还是有很多点幺注意的。
     
     重点：[left, right], [left, right） impacts: 1. right的取值， 2， while的判断， 3， if（nums[mid]>target), right的取值。
     

27. 移除元素
    题目建议： 暴力的解法，可以锻炼一下我们的代码实现能力，建议先把暴力写法写一遍。 双指针法 是本题的精髓，今日需要掌握，至于拓展题目可以先不看。
    
    题目链接：https://leetcode.cn/problems/remove-element/
    
    文章讲解：https://programmercarl.com/0027.%E7%A7%BB%E9%99%A4%E5%85%83%E7%B4%A0.html
    
    视频讲解：https://www.bilibili.com/video/BV12A4y1Z7LP 
    
    题目：https://leetcode.com/problems/remove-element/
    
    看到题目的第一想法： 心里有一定想法，但想看完视频讲解才开始做题。原来心中的想法是暴力解题法。看了视频才知道有双指针法。
     
    实现过程中遇到哪些困难: 暴力解题法：还是靠debug发现了问题，问题1. i的位置，会因为前置了数据，而应该减少，问题2.需要历遍数组的长度应该减少
     
    看完代码随想录之后的想法: 
     
    今日收获：
     
    重点：
