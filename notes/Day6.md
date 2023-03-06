6 第三章 哈希表

● day 1 任务以及具体安排：https://docs.qq.com/doc/DUG9UR2ZUc3BjRUdY  

● day 2 任务以及具体安排：https://docs.qq.com/doc/DUGRwWXNOVEpyaVpG  

● day 3 任务以及具体安排：https://docs.qq.com/doc/DUGdqYWNYeGhlaVR6 

● day 4 任务以及具体安排：https://docs.qq.com/doc/DUFNjYUxYRHRVWklp 


 今日任务 

● 哈希表理论基础

● 242.有效的字母异位词 

● 349. 两个数组的交集 

● 202. 快乐数

● 1. 两数之和   


 详细布置 

 哈希表理论基础 

建议：大家要了解哈希表的内部实现原理，哈希函数，哈希碰撞，以及常见哈希表的区别，数组，set 和map。  

**数值做映射：长度固定
set：长度比较长
map：key有value**

什么时候想到用哈希法，**当我们遇到了要快速判断一个元素是否出现在集合里的时候，就要考虑哈希法**。  这句话很重要，大家在做哈希表题目都要思考这句话。 

文章讲解：https://programmercarl.com/%E5%93%88%E5%B8%8C%E8%A1%A8%E7%90%86%E8%AE%BA%E5%9F%BA%E7%A1%80.html  


 242.有效的字母异位词 

建议： 这道题目，大家可以感受到 数组 用来做哈希表 给我们带来的遍历之处。 

题目链接/文章讲解/视频讲解： https://programmercarl.com/0242.%E6%9C%89%E6%95%88%E7%9A%84%E5%AD%97%E6%AF%8D%E5%BC%82%E4%BD%8D%E8%AF%8D.html  

视频讲解： 

题目：https://leetcode.com/problems/valid-anagram/

看到题目的第一想法：直接看视频。

实现过程中遇到哪些困难: string s.**charAt(index)**

看完代码随想录之后的想法:  一共26个字母，可以int[26]，然后对应下数组位置，可以mark出现过的。==》 没想到是，第一遍是对应位置mark ++，第二遍是对应位置mark --，最后一遍是判断是否有不为零的情况。

今日收获： 字母相对位置可以用 t[s.chartAt(index) **-'a'**]; 

重点：数组用在哈希法。 表的大小是固定而且不多的时候


 349. 两个数组的交集 

建议：本题就开始考虑 什么时候用set 什么时候用数组，本题其实是使用set的好题，但是后来力扣改了题目描述和 测试用例，添加了 0 <= nums1[i], nums2[i] <= 1000 条件，所以使用数组也可以了，不过建议大家忽略这个条件。 尝试去使用set。 

题目链接/文章讲解/视频讲解：https://programmercarl.com/0349.%E4%B8%A4%E4%B8%AA%E6%95%B0%E7%BB%84%E7%9A%84%E4%BA%A4%E9%9B%86.html  

视频讲解： https://www.bilibili.com/video/BV1ba411S7wu/

题目：https://leetcode.com/problems/intersection-of-two-arrays

看到题目的第一想法：时间关系， 还是看视频吧。

实现过程中遇到哪些困难: 1. hashset如何转换成int[]

看完代码随想录之后的想法: 看了视频后，比较迅速地做出来。

今日收获：resultSet.stream().mapToInt(**x->x**).toArray() === resultSet.stream().mapToInt(Integer::IntValue).toArray()

重点：hashSet.add(value); hashSet.contains(value); 一些数是否在某集合里面出现过 =》 哈希表

 202. 快乐数 

建议：这道题目也是set的应用，其实和上一题差不多，就是 套在快乐数一个壳子 

题目链接/文章讲解：https://programmercarl.com/0202.%E5%BF%AB%E4%B9%90%E6%95%B0.html 

视频讲解： N/A

题目：https://leetcode.com/problems/happy-number

看到题目的第一想法：完全没有想到如何实现。

实现过程中遇到哪些困难: 看了题解还是没有明白。最后是debug了code，再看回题解，才明白要点

看完代码随想录之后的想法: 还是得好好想想，怎样用好哈希表。

今日收获：1. 哈希表，要判断一个元素是否出现在集合里面，可以考虑哈希法。

2. int n 取每个digit =》while(n>0) {print(n % 10)， n = n/10};

重点：题目中说了会 无限循环，那么也就是说求和的过程中，**sum会重复出现，这对解题很重要**！

正如：关于哈希表中所说，当我们遇到了要快速判断一个元素是否出现集合里的时候，就要考虑哈希法了。

所以这道题目使用哈希法，来**判断这个sum是否重复出现，如果重复了就是return false， 否则一直找到sum为1为止**。

 1. 两数之和 

建议：本题虽然是 力扣第一题，但是还是挺难的，也是 代码随想录中 数组，set之后，使用map解决哈希问题的第一题。 

建议大家先看视频讲解，然后尝试自己写代码，在看文章讲解，加深印象。 

题目链接/文章讲解/视频讲解：https://programmercarl.com/0001.%E4%B8%A4%E6%95%B0%E4%B9%8B%E5%92%8C.html 

视频讲解： https://www.bilibili.com/video/BV1aT41177mK

题目：https://leetcode.com/problems/two-sum/

看到题目的第一想法：我之前应该做过， 希望能回想起来，可惜没有。看了solution，才有点感觉，然后试做一下，大体能找到思路，就是没有想到，最后的结果不是从map里面拿去，而是需要新创造int【2】，结果一个是当前的值的位置，另外一个才是从map里面拿出来。

实现过程中遇到哪些困难: 没有想到为什么要用hashset。后来看视频才了解到，若是搜索之前在一堆数里面有没有出现过，就是应该用hashset

看完代码随想录之后的想法: 很多细节，需要注意，特别是怎样可以用到hashset/hashmap/array，在什么情况下，分别用哪一种。

今日收获：重新刷了一次梦的开始，也是噩梦的开始。

重点：map，定义key和value。 key可以是用数组的值，value可以是数组的下标，看题目究竟是想返回的是什么。
