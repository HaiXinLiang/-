day 13 第五章 栈与队列 
 今日内容： 

● 239. 滑动窗口最大值

● 347.前 K 个高频元素

● 总结

 
 详细布置 


 239. 滑动窗口最大值 （一刷至少需要理解思路）

之前讲的都是栈的应用，这次该是队列的应用了。

本题算比较有难度的，需要自己去构造单调队列，建议先看视频来理解。 

题目链接/文章讲解/视频讲解：https://programmercarl.com/0239.%E6%BB%91%E5%8A%A8%E7%AA%97%E5%8F%A3%E6%9C%80%E5%A4%A7%E5%80%BC.html 


视频讲解：https://www.bilibili.com/video/BV1XS4y1p7qj

题目：https://leetcode.com/problems/sliding-window-maximum

看到题目的第一想法： 

实现过程中遇到哪些困难: 完全没有想过自己构造一个class出来实现功能。

看完代码随想录之后的想法: 看了视频再做，感觉有点模糊，但算是做出来了。

今日收获：再次深入认识Deque，原来它可以用作stack，也当然是queue，双向的。

重点：class MyQueue的构造，还有窗口的移动
for(int i = k; i<nums.length;i++){
            **myQueue.poll(nums[i-k]);
            myQueue.add(nums[i]);**
            result[num++] = myQueue.getMaxValue();
        }

 347.前 K 个高频元素  （一刷至少需要理解思路）

大/小顶堆的应用， 在C++中就是优先级队列 (MaxHeap, MinHeap)

本题是 大数据中取前k值 的经典思路，了解想法之后，不算难。

题目链接/文章讲解/视频讲解：https://programmercarl.com/0347.%E5%89%8DK%E4%B8%AA%E9%AB%98%E9%A2%91%E5%85%83%E7%B4%A0.html  

视频讲解：https://www.bilibili.com/video/BV1Xg41167Lz

题目：https://leetcode.com/problems/top-k-frequent-elements

看到题目的第一想法： 原来2021年做过的题目，完全没有印象呢。当时用了两三种方法实现，一个是用java 8 的lambda， 一个是用priorityQueue, 还有用ArrayList.现在再看，只有前两个看得懂。。。

实现过程中遇到哪些困难: 对priorityQueue完全空白，恶补了几个视频。

看完代码随想录之后的想法: 看了视频再做，理解了思路，但是对大堆栈，小堆栈没有任何概念。 得看着code，边参考边写出来。

今日收获：认识priorityQueue很好玩，后面需要加强comparator的认识。

重点: map.put(num, **map.getOrDefault(num, 0)**+1);
 
 PriorityQueue<**Int[]**> pq = new PriorityQueue<>(**(a, b) -> a[1] - b[1]**); MinHeap
 PriorityQueue<**Int[]**> pq = new PriorityQueue<>(**(a, b) -> b[1] - a[1]**);  MaxHeap
 
 PriorityQueue<**Map.Entry<Integer, Integer>**> pq = new PriorityQueue<>(**Comparator.comparingInt(Map.Entry::getValue)**); MaxHeap


 总结 

栈与队列做一个总结吧，加油

https://programmercarl.com/%E6%A0%88%E4%B8%8E%E9%98%9F%E5%88%97%E6%80%BB%E7%BB%93.html  
