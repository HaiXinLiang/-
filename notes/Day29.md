第七章 回溯算法part05


* 491.递增子序列

* 46.全排列

* 47.全排列 II

详细布置 

491.递增子序列 

本题和大家刚做过的 90.子集II 非常像，但又很不一样，很容易掉坑里。 
https://programmercarl.com/0491.%E9%80%92%E5%A2%9E%E5%AD%90%E5%BA%8F%E5%88%97.html 

视频讲解：https://www.bilibili.com/video/BV1EG4y1h78v  

题目：https://leetcode.com/problems/non-decreasing-subsequences

看到题目的第一想法：以为自己可以做出来。结果，一没有看清题目 **return all the different possible non-decreasing subsequences**， 二是套用那树层去重是boolean[] used，之前是得是sort数组后用，没有sort不能用 

实现过程中遇到哪些困难: 1.是返回组合是非递减数组 2. 用map来去重，同一父节点下同一层的去重
![image](https://user-images.githubusercontent.com/87255377/228519628-8eb59964-cdc1-441a-ad3c-9679e84adc9f.png)


看完代码随想录之后的想法:

今日收获：

重点：

46.全排列 
本题重点感受一下，排列问题 与 组合问题，组合总和，子集问题的区别。 为什么排列问题不用 startIndex 
https://programmercarl.com/0046.%E5%85%A8%E6%8E%92%E5%88%97.html   

视频讲解：https://www.bilibili.com/video/BV19v4y1S79W  

题目：https://leetcode.com/problems/permutations

看到题目的第一想法：没有做出来，没想到用used来记录，已经取过的元素。
![image](https://user-images.githubusercontent.com/87255377/228527797-bc24af59-dde1-4043-a666-1db97670c60f.png)

实现过程中遇到哪些困难: 没有想到如何skip已经取过的元素。看了视频后才发现要点。

看完代码随想录之后的想法:

今日收获：

重点：用used记录已经取过的元素，以达到skip那些取过元素的目的

47.全排列 II 
本题 就是我们讲过的 40.组合总和II 去重逻辑 和 46.全排列 的结合，可以先自己做一下，然后重点看一下 文章中 我讲的拓展内容。 used[i - 1] == true 也行，used[i - 1] == false 也行 

https://programmercarl.com/0047.%E5%85%A8%E6%8E%92%E5%88%97II.html     
 
视频讲解：https://www.bilibili.com/video/BV1R84y1i7Tm

题目：https://leetcode.com/problems/permutations-ii

看到题目的第一想法：应该可以自己独立做出来

实现过程中遇到哪些困难: 看完题目，写code前，让自己记得sort了那数组再做backtracking，结果一下子忘了，run test case的时候报错，才发现错误。 还好一下子修正过来。

看完代码随想录之后的想法:

今日收获：真的做出来了，yeah！而且跟标准答案相差不多

重点：
