8 第四章 字符串

 今日任务 

● 344.反转字符串

● 541. 反转字符串II

● 剑指Offer 05.替换空格

● 151.翻转字符串里的单词

● 剑指Offer58-II.左旋转字符串


 详细布置 

 344.反转字符串 

建议： 本题是字符串基础题目，就是考察 reverse 函数的实现，同时也明确一下 平时刷题什么时候用 库函数，什么时候 不用库函数 

题目链接/文章讲解/视频讲解：https://programmercarl.com/0344.%E5%8F%8D%E8%BD%AC%E5%AD%97%E7%AC%A6%E4%B8%B2.html  


视频讲解： 

题目：

看到题目的第一想法：看到很熟悉，然后试做一下有点乱，再看了一下视频，确认了自己的想法是正确的解题思路。

实现过程中遇到哪些困难: 一下子做出来了。

看完代码随想录之后的想法: 确认了自己的想法是正确的解题思路。

今日收获：

重点：继续双指针

 541. 反转字符串II

建议：本题又进阶了，自己先去独立做一做，然后在看题解，对代码技巧会有很深的体会。 

题目链接/文章讲解/视频讲解：https://programmercarl.com/0541.%E5%8F%8D%E8%BD%AC%E5%AD%97%E7%AC%A6%E4%B8%B2II.html  


视频讲解： 

题目：

看到题目的第一想法：希望自己能做出来，结果没有。

实现过程中遇到哪些困难: 试了很久，都没有做出来，看了视频，才了解思路。

看完代码随想录之后的想法: 看了视频发现是1. 应该分段处理，如何分段是个巧妙的地方i+=2*k, 2.原来reverse还可以就start和end的index，来对中间的数组reverse。

今日收获：加深了reverse，不单单只是整个数组的reverse，对于中间也可以reverse。

重点：1. 首先是for(int i=o;i<ch.length;**i+=2k**), 
2. string -> char => char[] ch = s.toCharArray(), char -> string => new String(ch)
3. reverse的ending确定Math.min(**s.length-1**, **start + k - 1**);


 剑指Offer 05.替换空格 

建议：对于线性数据结构，填充或者删除，后序处理会高效的多。好好体会一下。
题目链接/文章讲解：https://programmercarl.com/%E5%89%91%E6%8C%87Offer05.%E6%9B%BF%E6%8D%A2%E7%A9%BA%E6%A0%BC.html  


视频讲解： 

题目：

看到题目的第一想法：我试着用char[] = s.toCharArray();然后replace；最后发现char[]是固定长度呢~【汗颜】

实现过程中遇到哪些困难: 

看完代码随想录之后的想法: 最后用来StringBuilder来实现，但是还是没有时间好好体会一把后序处理，有时间今天再看看。

今日收获：StringBuilder

重点：


 151.翻转字符串里的单词 

建议：这道题目基本把 刚刚做过的字符串操作 都覆盖了，不过就算知道解题思路，本题代码并不容易写，要多练一练。 

题目链接/文章讲解/视频讲解：https://programmercarl.com/0151.%E7%BF%BB%E8%BD%AC%E5%AD%97%E7%AC%A6%E4%B8%B2%E9%87%8C%E7%9A%84%E5%8D%95%E8%AF%8D.html 

视频讲解： 

题目：

看到题目的第一想法：希望自己能做出来，结果没有。

实现过程中遇到哪些困难:看了视频，才了解思路。

看完代码随想录之后的想法: 不是一般的繁琐，要分成3部分完成，一是trim多余的spaces，二是整个string反转，然后是每个word反转。

今日收获：好在整个string的反转和每个word的反转都可以套用一个程序来实现。

重点：char[] 剪短 =》 System.arraycopy(originalChars, start_index, newChars, start_index, length)
char -> string => new String(ch)

 剑指Offer58-II.左旋转字符串 

建议：题解中的解法如果没接触过的话，应该会想不到

题目链接/文章讲解：https://programmercarl.com/%E5%89%91%E6%8C%87Offer58-II.%E5%B7%A6%E6%97%8B%E8%BD%AC%E5%AD%97%E7%AC%A6%E4%B8%B2.html  


视频讲解： N/A

题目：

看到题目的第一想法：

实现过程中遇到哪些困难: 自己用了System.arraycopy实现的，创建了另外一个array出来，

看完代码随想录之后的想法: 看文章，发现karl思路是用的是反转再反转。

今日收获：起码自己做出来了，但是没有用今天所学的来做，也没有用到最快的方法做出来，

重点:看到题解，最快的是用subString()
