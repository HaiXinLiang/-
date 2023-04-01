第八章 贪心算法 part01


● 理论基础 

● 455.分发饼干 

● 376. 摆动序列 

● 53. 最大子序和 

贪心算法其实就是没有什么规律可言，所以大家了解贪心算法 就了解它没有规律的本质就够了。 

不用花心思去研究其规律， 没有思路就立刻看题解。

基本贪心的题目 有两个极端，要不就是特简单，要不就是死活想不出来。  

学完贪心之后再去看动态规划，就会了解贪心和动规的区别。

详细布置 

理论基础 

https://programmercarl.com/%E8%B4%AA%E5%BF%83%E7%AE%97%E6%B3%95%E7%90%86%E8%AE%BA%E5%9F%BA%E7%A1%80.html  

视频：https://www.bilibili.com/video/BV1WK4y1R71x

455.分发饼干  

https://programmercarl.com/0455.%E5%88%86%E5%8F%91%E9%A5%BC%E5%B9%B2.html  

视频： https://www.bilibili.com/video/BV1MM411b7cq/

题目：https://leetcode.com/problems/assign-cookies/

看到题目的第一想法：对贪心算法还是有些模糊

实现过程中遇到哪些困难: 我用饼干去遍历了，如果先考虑大饼干去喂饱小饼干，应该用胃口作为for遍历，因为for遍历的i位置是不断减少，不可控制。但在for循环里面的if条件是可以控制饼干的位置。

看完代码随想录之后的想法:

今日收获：第一道贪心算法完败。收获是for的特性，i位置是不断减少，if条件是可控位置。

重点：

376. 摆动序列  

https://programmercarl.com/0376.%E6%91%86%E5%8A%A8%E5%BA%8F%E5%88%97.html 

视频： https://www.bilibili.com/video/BV17M411b7NS

题目：https://leetcode.com/problems/wiggle-subsequence

看到题目的第一想法：直接看视频了

实现过程中遇到哪些困难: 很容易忽略单调中间有平坡的情况，而且感觉不容易出来。看了视频知道怎么处理，多看一遍视频才知道原理是prediff没有必要跟着currdiff走，它只需要有摆动的时候才记录下当前prediff的方向。

看完代码随想录之后的想法:

今日收获：贪心没套路，有点跟不上。加油！！！

重点：

53. 最大子序和  

https://programmercarl.com/0053.%E6%9C%80%E5%A4%A7%E5%AD%90%E5%BA%8F%E5%92%8C.html  

视频： https://www.bilibili.com/video/BV1aY4y1Z7ya

题目：https://leetcode.com/problems/maximum-subarray

看到题目的第一想法：看了视频后，了解思路，debug了好些次，自己做出来了。

实现过程中遇到哪些困难: result的更新是result与前连续和两者间取最大值。自己没有在连续和改变后，及时更新result数值

看完代码随想录之后的想法:

今日收获：还是得多思考呀。即使看了视频了解思路，也得多想想。

重点：
