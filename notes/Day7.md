7 第三章 哈希表 

 今日任务 

● 454.四数相加II 

● 383. 赎金信 

● 15. 三数之和 

● 18. 四数之和 

● 总结  

 详细布置 

 454.四数相加II 

建议：本题是 使用map 巧妙解决的问题，好好体会一下 哈希法 如何提高程序执行效率，降低时间复杂度，当然使用哈希法 会提高空间复杂度，但一般来说我们都是舍空间 换时间， 工业开发也是这样。

题目链接/文章讲解/视频讲解：https://programmercarl.com/0454.%E5%9B%9B%E6%95%B0%E7%9B%B8%E5%8A%A0II.html  

视频讲解： https://www.bilibili.com/video/BV1Md4y1Q7Yh/

题目：https://leetcode.com/problems/4sum-ii/

看到题目的第一想法：时间关系， 还是看视频吧。

实现过程中遇到哪些困难: Java，没有这key的元素，对应的值是null。

看完代码随想录之后的想法: 没想到跟两数之和这么类似的解题过程。

今日收获：有两种做法对于没有Key的插入。 1. sumABMap.put(sumAB, sumABMap.get(sumAB) == null?1: sumABMap.get(sumAB)+1); 2. if (map.containsKey(temp)) 

重点：继续哈希


 383. 赎金信  

建议：本题 和 242.有效的字母异位词 是一个思路 ，算是拓展题 

题目链接/文章讲解：https://programmercarl.com/0383.%E8%B5%8E%E9%87%91%E4%BF%A1.html 

视频讲解： N/A

题目：https://leetcode.com/problems/ransom-note/

看到题目的第一想法：跟昨天那道题目超级相像。

实现过程中遇到哪些困难: 几乎没有遇到困难。只是把求String的长度，数组的长度，还有。。。的长度混乱了。。

看完代码随想录之后的想法:跟自己写的一样，太骄傲了。

今日收获：超级鸡血，凭自己的力量做出来。没有看视频。证明昨天的学习，正真吸收了。开心！

重点：charAt(i) - 'a' 定数组下标


 15. 三数之和 

建议：本题虽然和 两数之和 很像，也能用哈希法，但用哈希法会很麻烦，双指针法才是正解，可以先看视频理解一下 双指针法的思路，文章中讲解的，没问题 哈希法很麻烦。 

题目链接/文章讲解/视频讲解：https://programmercarl.com/0015.%E4%B8%89%E6%95%B0%E4%B9%8B%E5%92%8C.html 

视频讲解： https://www.bilibili.com/video/BV1GW4y127qo

题目：https://leetcode.com/problems/3sum/

看到题目的第一想法：时间关系， 还是看视频吧。

实现过程中遇到哪些困难: 去重的问题，怎样去重，在哪里去重比较好。而且当==0 的时候，忘了left++及right--了

看完代码随想录之后的想法:去重比较难，特别是left和right的去重。

今日收获：看了一下别人的答案，有些人是用set来存储结果集，所以就自动去重了，66666.试了一下，Set耗时长。

重点：如何去重，在哪里去重。还有在==0的时候，不要忘了left++及right--

 18. 四数之和  

建议： 要比较一下，本题和 454.四数相加II 的区别，为什么 454.四数相加II 会简单很多，这个想明白了，对本题理解就深刻了。 本题 思路整体和 三数之和一样的，都是双指针，但写的时候 有很多小细节，需要注意，建议先看视频。 

题目链接/文章讲解/视频讲解：https://programmercarl.com/0018.%E5%9B%9B%E6%95%B0%E4%B9%8B%E5%92%8C.html 

视频讲解： https://www.bilibili.com/video/BV1DS4y147US

题目：https://leetcode.com/problems/4sum/

看到题目的第一想法：时间关系， 还是看视频吧。

实现过程中遇到哪些困难: 在三数之和的基础上改code还是比较容易做出来的。难点是k和i的减去枝条。我开始没想过要减枝的，感觉没有必要，有就更好而已。原来不是。

看完代码随想录之后的想法: 四数之和真的是三数之和的加强版~~ 6666

今日收获：resultIntegerList.add(Arrays.asList(nums[k],nums[i],nums[left], nums[right]));

重点：去枝 if(nums[k] > 0 && nums[k] > target) break; 
if(nums[k] + nums[i]> 0 && nums[k] + nums[i] > target) break;
