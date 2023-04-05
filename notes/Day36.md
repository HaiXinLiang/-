第八章 贪心算法 part05

● 435. 无重叠区间 

● 763.划分字母区间 

● 56. 合并区间 

 详细布置  

今天的三道题目，都算是 重叠区间 问题，大家可以好好感受一下。 都属于那种看起来好复杂，但一看贪心解法，惊呼：这么巧妙！ 
还是属于那种，做过了也就会了，没做过就很难想出来。
不过大家把如下三题做了之后， 重叠区间 基本上差不多了

 435. 无重叠区间 

https://programmercarl.com/0435.%E6%97%A0%E9%87%8D%E5%8F%A0%E5%8C%BA%E9%97%B4.html  

视频：https://www.bilibili.com/video/BV1A14y1c7E1

题目：https://leetcode.com/problems/non-overlapping-intervals

看到题目的第一想法：自己可以做出来。

实现过程中遇到哪些困难: 区间重叠的判断一开始不是太准确，debug后修改了，自己做出来了。

看完代码随想录之后的想法:

今日收获：

重点：

 763.划分字母区间 

https://programmercarl.com/0763.%E5%88%92%E5%88%86%E5%AD%97%E6%AF%8D%E5%8C%BA%E9%97%B4.html  

视频：https://www.bilibili.com/video/BV18G4y1K7d5

题目: https://leetcode.com/problems/partition-labels/

看到题目的第一想法：不是太会做，看了视频，知道了原理。

实现过程中遇到哪些困难: 自己写代码，哈希数组用了，但是不会怎样遍历，才能把功能实现出来。隐隐约约知道，要取最大值，和 i==最大值的时候，就是划分区间的时候。

看完代码随想录之后的想法:

今日收获：

重点：

 56. 合并区间  
本题相对来说就比较难了。

https://programmercarl.com/0056.%E5%90%88%E5%B9%B6%E5%8C%BA%E9%97%B4.html  

视频：https://www.bilibili.com/video/BV1wx4y157nD

题目：https://leetcode.com/problems/merge-intervals/

看到题目的第一想法：应该可以做出来，结果没有

实现过程中遇到哪些困难: 合并了两个，但是没有合并三个重叠的55555

看完代码随想录之后的想法:要不断更新边界！！！！！血的教训！ 而不是直接把元素塞在result里面然后就不动了。

今日收获：

重点：
