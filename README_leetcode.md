# Code

This is an old file to help me get familiar with leetcode questions. However, after I have practiced 200 questions, I have known pretty much of the basics to make the code done. So I stop to update this file. I only add new tips and also include some hard or interesting coding questions into the ["README.md"](./README.md) file

Learning the coding day by day. 
---

这里仅仅是学习算法前期的一些题目，当时为了督促自己刷题，每刷一题的时候都会记录，帮助回忆一下这个题目的要点难点，知识点等等。刷到200题目的时候发现很多题目其实练习的意义不大。大多数题目都很相似，或者也有很简单的，每次都把题目标题拷贝下来用处不大。因此后面的题目并没有具体分析。但是java文件中依然会记录一些题目的思路和要点。欢迎参考，提出建议。

--

[128. Longest Consecutive Sequence](https://leetcode.com/problems/longest-consecutive-sequence/?tab=Description) 
  complexity of HashMap/HashSet ~ O(1)
  利用HashMap存储每个位置的连通的个数。在HashMap中，每次只需要连通数组两端的统计值，其余的值在循环中将不在用到，因此不需要更新。
  

[445. Add Two Numbers II](https://leetcode.com/problems/add-two-numbers-ii/)
  通过链表的方式实现两个整数的相加。利用stack存储链表，每次提取出最后一位相加，最后存储在链表中。


[148. Sort List](https://leetcode.com/problems/sort-list/) 两种思路实现链表的排序，merge sort 和 quick sort。 用递归完成归并排序程序非常简洁，很好理解。

[147. Insertion Sort List](https://leetcode.com/problems/insertion-sort-list/) 用insertion sort的方法对链表进行排序, 复杂度O(n^2), 注意对链表的排序并没有意义，速度太慢。

[328. Odd Even Linked List](https://leetcode.com/problems/odd-even-linked-list/) 与147的思路一样，考虑的是链表的基本操作。注意的是不要使用暴力的奇偶节点直接相加的方法，可以只把后面偶数节点放在前面，最后循环后将偶数节点放在奇数节点后。	
>所有链表题目注意保存最初节点位置，保存的数目跟最后需要返回的节点数目有关。

[88. Merge Sorted Array](https://leetcode.com/problems/merge-sorted-array/?tab=Solutions) 简单题，考虑的merger排序的基本过程。
>一般题目都是变种题，在特定的环境下，结题方法都会有改进的空间。这一题中直接在数组nums1中操作即可，不需要额外空间。

[19. Remove Nth Node From End of List
](https://leetcode.com/problems/remove-nth-node-from-end-of-list/) 用双指针操作链表。思路比较巧，难度不大。

[61. Rotate List
](https://leetcode.com/problems/rotate-list/) 难度不大，巧妙。将链表改变为环形链表然后移动。


[125. Valid Palindrome
](https://leetcode.com/problems/valid-palindrome/?tab=Solutions) 简单题，判断回文字符串。使用字符数字判断函数Character.isLetterOrDigit()。还有一个[简洁解法](125_easySolution.java)，不过调用了库函数。

[9. Palindrome Number](https://leetcode.com/problems/palindrome-number/?tab=Solutions) 回文数字的判断，注意情况的判断，有一定的tricky。

[234. Palindrome Linked List](https://leetcode.com/problems/palindrome-linked-list/?tab=Solutions) 在O(n)的时间复杂度下判断链表的回文情况，这里用到了快慢指针，注意考虑指针的数目和指针的多少。运用到了链表的reverse。

[25. Reverse Nodes in k-Group](https://leetcode.com/problems/reverse-nodes-in-k-group/?tab=Solutions) 递归的指针操作。思想不难，体会到了递归的困难之处。用递归结题时请考虑好每次递归的初始条件输出条件。其实一般程序都应如此。

[400. Nth Digit](https://leetcode.com/problems/nth-digit/?tab=Description) 思想不难，算准很难。还有溢出问题需要考虑。

[221. Maximal Square](https://leetcode.com/problems/maximal-square/?tab=Solutions) 动态规划练手，注意矩阵大小的初始化。

[112. Path Sum](https://leetcode.com/problems/path-sum/?tab=Solutions) 二叉树，递归求解即可

[230. Kth Smallest Element in a BST](https://leetcode.com/problems/kth-smallest-element-in-a-bst/?tab=Solutions) 二叉树，递归求解训练好题 

[385. Mini Parser](https://leetcode.com/problems/mini-parser/?tab=Description) 练习堆栈的好题，容易出错。 

	> recursion 和 stack 方法往往是可以相互转化的
	
[67. Add Binary](https://leetcode.com/problems/add-binary/?tab=Solutions) string练手题目。字符与数字的相关操作。

> Integer.parseInt(string)	
>  int i = Integer.valueOf(my_str).intValue();	
> StringBuilder s = new StringBuilder();	
> s.reverse().toString();	
> String s = String.valueOf(i);	
> String s = Integer.toString(i);	
> String s = "" + i;	

[64. Minimum Path Sum](https://leetcode.com/problems/minimum-path-sum/?tab=Description) 动态规划简单题，直接练手。

[22. Generate Parentheses](https://leetcode.com/problems/generate-parentheses/?tab=Solutions) 找出所有可能的正反括号组合，使用递归方法求解，由下而上的思路。

[49. Group Anagrams](https://leetcode.com/problems/anagrams/?tab=Description) 字符串可以使用下面的语句来完成排序。
           
>char[] c = s.toCharArray();	
>arrays.sort(c);

python 里面也有快速排序字符串的程序

> "".join(sorted(s))
> list(s)

[71. Simplify Path](https://leetcode.com/problems/simplify-path/) 将路径转化成绝对路径。注意考虑corner case 多测试。

[3. Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/?tab=Solutions) 找到字符串中最长子字符串的长度，非常好的string练习题。可以有的思想包括：
> 二分法	
> DP法	
> 双指针法	

[43. Multiply Strings](https://leetcode.com/problems/multiply-strings/?tab=Solutions) 完成两个长整数字符串的相加。

[91. Decode Ways](https://leetcode.com/problems/decode-ways/?tab=Solutions) 用动态规划解决，注意0 的情况。

[151. Reverse Words in a String](https://leetcode.com/problems/reverse-words-in-a-string/?tab=Solutions) 完成字符串中单词的翻转。不适用API的情况下可以用stack结构完成，也可以使用从后往前读取字符串的方式完成。还可以考虑**翻转整个字符串**的方式。

[214. Shortest Palindrome](https://leetcode.com/problems/shortest-palindrome/?tab=Solutions) 修改字符串达到最小回文字符串，暴力解法不难，但是需要注意边界情况。开始没有处理好完全没有回文字符串的情况。另外时间复杂度可以优化，通过[KMP方法](https://discuss.leetcode.com/topic/27261/clean-kmp-solution-with-super-detailed-explanation)。代码简洁度可以优化，例如用[递归的方法](https://discuss.leetcode.com/topic/21068/my-7-lines-recursive-java-solution)

[503. Next Greater](https://leetcode.com/problems/next-greater-element-ii/?tab=Description) 维护一个最小栈结构，注意corner case的考虑。

[451. Sort Characters By Frequency](https://leetcode.com/problems/sort-characters-by-frequency/?tab=Solutions) 计数问题可以想到用HashMap来快速记录和读取每个元素出现的个数。用bucket sort的方法来对计数问题进行快速排序。

[150. Evaluate Reverse Polish Notation](https://leetcode.com/problems/evaluate-reverse-polish-notation/?tab=Solutions) 用栈结构即可解决。注意处理运算次序问题。**每次写完程序请跑一下test case**

[373. Find K Pairs with Smallest Sums](https://leetcode.com/problems/find-k-pairs-with-smallest-sums/?tab=Description) 注意一系列的TOP K 的问题，解法很类似。考虑哈希堆，最大/小堆。**熟练代码**

[263. Ugly Number](https://leetcode.com/problems/ugly-number/?tab=Description) 判断是否为ugly number, 注意考虑后续问题。

[475. Heaters](https://leetcode.com/problems/heaters/#/solutions) 应用二分查找法，或者直接暴力查找。很好的corner case 的练习

[278. First Bad Version](https://leetcode.com/problems/first-bad-version/#/solutions) 二分法的基础训练，注意位移操作优先级低于加减符号，高于大于小于号。二分法注意指标corner case

[74. Search a 2D Matrix](https://leetcode.com/problems/search-a-2d-matrix/#/description) 初级二分法题目。[二分法总结](https://mp.weixin.qq.com/s?__biz=MzAwMDk1MTUyNw==&mid=2247484110&idx=3&sn=c6403ffc79f278affcdf651e7ed8437e&chksm=9ae05746ad97de50a131c586272a6ab2a6dbb19186c0e92aa387c61d725db7d367e18df0614e&mpshare=1&scene=1&srcid=03149mRY4cn1dmyw7hDfpGeL&key=32ff7e6b073562f957522cfd39539c30bdab6c9beb05ffbb79eec8be5bf9b2b23a3cb866ef0467bef8684a002f1bb925b1fd4f0a810089352a9ca5cb4a5eb68f7d015d05b303378b3274313d8ab8a479&ascene=0&uin=NzIzOTQyODAx&devicetype=iMac+MacBookPro11%2C1+OSX+OSX+10.9.5+build(13F1911)&version=11020201&pass_ticket=usXZy7VMRtnoFNo4bPHKthdhL%2FjUpdAOJ1iPEB8Q61r6cM3KmbHGv35B3YiNFjXS)

[153. Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/#/description) 采用标准的二分法模板结题，好处是每次不用为边界的条件考虑太多，只是最终的代码行数会多一点点。

[78. subsets](https://leetcode.com/problems/subsets/#/solutions) 回溯法 backtrack。该题需要练习

[435. Non-overlapping Intervals](https://leetcode.com/problems/non-overlapping-intervals/#/description) 问题的本质是查找overlap的数目，这时候需要考虑到底有多少中overlap的情况。主要想到先排序比较难。

[452. Minimum Number of Arrows to Burst Balloons](https://leetcode.com/problems/minimum-number-of-arrows-to-burst-balloons/#/description) 贪心算法的基本题型，注意考虑的是原始数据排序是递增和递减的情况

[321. Create Maximum Number](https://leetcode.com/problems/create-maximum-number/#/description)  hard难度，适合练习！！重新练习

[179. Largest Number](https://leetcode.com/problems/largest-number/#/solutions) 思路的思考

[324. Wiggle Sort I]() O(n)算法，简单循环即可。

[324. Wiggle Sort II](https://leetcode.com/problems/wiggle-sort-ii/#/solutions) 快排+index mapping，重新读代码，难度略大。

[102. Binary Tree Level Order Traversal I](https://leetcode.com/problems/binary-tree-level-order-traversal/#/solutions) DFS BFS 

[107. Binary Tree Level Order Traversal II](https://leetcode.com/problems/binary-tree-level-order-traversal-ii/#/description)  DFS BFS 必须练习题目. Given a binary tree, return the bottom-up level order traversal of its nodes' values. (ie, from left to right, level by level from leaf to root).
> 这个题目很简单，是练习DFS BFS必备技能

[542. 01 Matrix](https://leetcode.com/problems/01-matrix/#/description) BFS DFS 的题目，想思路的时候需要一点点分析。实现的时候遇到新的细节问题。

[101. Symmetric Tree](https://leetcode.com/problems/symmetric-tree/#/description) 检查树的对称性，简单题。用BFS的时候注意每次进和出两个node。

[513.Find Bottom Left Tree Value](https://leetcode.com/problems/find-bottom-left-tree-value/#/solutions) BFS  短小练习题，需要注意对队列操作细微变种。

[543. Diameter of Binary Tree](https://leetcode.com/problems/diameter-of-binary-tree/#/description) DFS recurrence，短小的练习题

[538. Convert BST to Greater Tree](https://leetcode.com/problems/convert-bst-to-greater-tree/#/description) Tree 的遍历，不难，注意corner case。如何增加class的变量来传递输出值。

[515. Find Largest Value in Each Tree Row](https://leetcode.com/problems/find-largest-value-in-each-tree-row/#/description) Tree, BFS 速度完成题目。

[200. Number of Islands](https://leetcode.com/problems/number-of-islands/#/solutions) matrix, BFS, DFS. 典型面试题，可以使用class的变量传递参数

[344. Reverse String](https://leetcode.com/problems/reverse-string/#/description)
[541. Reverse String II](https://leetcode.com/problems/reverse-string-ii/#/description) 
[557. Reverse String III](https://leetcode.com/contest/leetcode-weekly-contest-27/problems/reverse-words-in-a-string-iii/) 
 请注意查看344题目solution的[分析](https://discuss.leetcode.com/topic/43296/java-simple-and-clean-with-explanations-6-solutions)。注意字符串的操作方法。

>s.length()  	
char[] chars = s.toCharArray();		
String.valueOf(chars);	

[349. Intersection of Two Arrays](https://leetcode.com/problems/intersection-of-two-arrays/#/solutions) 二分法，注意练习。	
[350. Intersection of Two Arrays II](https://leetcode.com/problems/intersection-of-two-arrays-ii/#/solutions) 关于类似的排序和二分法问题，有fowllowing question 需要仔细考虑。

[162. Find Peak Element](https://leetcode.com/problems/find-peak-element/#/solutions) 经典二分法题目，简单，但是需要足够重视掌握。

[303. Range Sum Query - Immutable](https://leetcode.com/problems/range-sum-query-immutable/#/solutions) 简单DP题目

[53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/#/solutions) 简单DP题目

[198. House Robber](https://leetcode.com/problems/house-robber/#/description) 练习DP动态规划的好题, 简单。

[121. Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/#/description) 从 O(N^2) 到 O(N) 的进化。
> 关于股票问题的相关总结 [见这里](https://sophiesongge.github.io/leetcode/2017/02/15/buy-sell-stock.html)

[122. Best Time to Buy and Sell Stock II](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-ii/#/description) 注意与实际股票的差异，实际是寻找波峰和波谷这样的最大最小子结构.

[123. Best Time to Buy and Sell Stock III](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iii/#/description) Hard的DP题目

>动态规划: 初始状态→│决策１│→│决策２│→…→│决策ｎ│→结束状态	
>贪心: 初始状态→│第一步最优解│→│第二步最优解│→…→│第n步最优解│→结束状态

>很多问题都可以用动态规划和贪心两种方法来解决, 比如著名的背包问题(这是宝宝大学时期的一个大作业, 至今印象深刻)。 相对来讲, 一般情况下, 贪心算法占的空间会小一点, 但是, 贪心算法并不能保证最终得到的是全局最优解。
>
> 每个问题拿到的时候请先用数学形式描述出来，这时候基本上暴力解法就差不多了。

[139. Word Break](https://leetcode.com/problems/word-break/#/description) 用DP方法分割字符。

[140. Word Break II](https://leetcode.com/problems/word-break-ii/#/description) DP问题， 这一题需要重新审查，HARD难度 重新联系。DFS。见[每日一题](https://mp.weixin.qq.com/s?__biz=MzAwMDk1MTUyNw==&mid=2247484710&idx=1&sn=4cd1f71258d64e365eb632bcea368ed4&chksm=9ae050aead97d9b886acc87e7af313a863416a790a6948d5a64093d535856fdb36d05615b26c&mpshare=1&scene=1&srcid=0327QGTsI4ihK0ZdhKOdCiTP&key=056e2b9cbd625ceac4870f519af30a3b4626083f30946a8c65aa942ad24d933b1b2da1246d4cbffcab2dcd3d3215df0012f42f2ddf5f201c2b0f3478030c9207c08c37cb6b1403db8a4bb11e56681ede&ascene=0&uin=NzIzOTQyODAx&devicetype=iMac+MacBookPro11%2C1+OSX+OSX+10.9.5+build(13F1911)&version=11020201&pass_ticket=4gxhVzKA%2FMbWwKr26bHjhhM19bLa1cgo%2Bf41rJB2OYlhuE2LC9F3uawL5YGsFRDj)

[70. climbing stairs](https://leetcode.com/problems/climbing-stairs/#/description) DP Fibonacci

[523. Continuous Subarray Sum](https://leetcode.com/problems/continuous-subarray-sum/#/description) DP, 

[304. Range Sum Query 2D](https://leetcode.com/problems/range-sum-query-2d-immutable/#/solutions) DP

[257. Binary Tree Path](https://leetcode.com/problems/binary-tree-paths/#/solutions) BFS DFS, corner case 得小心

[523. Continuous Subarray Sum](https://leetcode.com/problems/continuous-subarray-sum/#/solutions) DP解法跟暴力解法一样，需要用到一点点数学技巧。注意0的cornercase。

[486. Predict the Winner](https://leetcode.com/problems/predict-the-winner/#/description) 双人从数组里面以此取数，属于博弈问题。DP 矩阵的算法值得参考。请查看solution中的思路讲解。
[474. Ones and Zeroes](https://leetcode.com/problems/ones-and-zeroes/#/description) 

[98. Validate Binary Search Tree](https://leetcode.com/problems/validate-binary-search-tree/) 判断是否为二叉搜索树。

> 相关问题	
> [94. Binary Tree Inorder Traversal](https://leetcode.com/problems/binary-tree-inorder-traversal/#/description)		
> [230. Kth Smallest Element in a BST](https://leetcode.com/problems/kth-smallest-element-in-a-bst/#/description)		
> [98. Validate Binary Search Tree](https://leetcode.com/problems/validate-binary-search-tree/#/description)

[1. Two Sum](https://leetcode.com/problems/two-sum/#/description) 	
[167. Two Sum II](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/#/description)  思路一样，可以加入binary search		
[170. Two Sum III](https://discuss.leetcode.com/category/178/two-sum-iii-data-structure-design) [博客园](http://www.cnblogs.com/grandyang/p/5184143.html)  结构编程，考虑trade off			
[15. Three Sum](https://leetcode.com/problems/3sum/#/description) 采用twoSum子程序让结果更简洁			
[18. Four SUm](https://leetcode.com/problems/4sum/#/description)

[110. Balanced Binary Tree](https://leetcode.com/problems/balanced-binary-tree/#/solutions)	Tree, 分治。练习必备

> 题目可以运用到多重数据结构。包括hashmap，二分法，双指针。特别是在two sum II中可以用多重方法求解。leetcode 必练题目

[547. Friend Circles](https://leetcode.com/problems/friend-circles/#/description) union find 题目 练手必备
[261. Graph Valid Tree](https://discuss.leetcode.com/category/330/graph-valid-tree) union find 练习。如果是树的话，所有的节点必须是连接的，也就是说必须是连通图，而且不能有环，所以我们的焦点就变成了验证是否是连通图和是否含有环。[九章](http://www.jiuzhang.com/solutions/graph-valid-tree/)

[332. Reconstruct Itinerary](https://leetcode.com/problems/reconstruct-itinerary/#/solutions) 图, dfs。

[490. The Maze](http://www.cnblogs.com/grandyang/p/6381458.html)

[108.Convert Sorted Array to Binary Search Tree](https://leetcode.com/problems/convert-sorted-array-to-binary-search-tree/#/solutions) 简单题，递归求解，必须非常熟练。

[120. Triangle](https://leetcode.com/problems/triangle/#/description) 典型DP问题

[494. Target Sum](https://leetcode.com/problems/target-sum/#/description) DP。中等难度典型题。可以改写成subset sum 的问题

[416. Partition Equal Subset Sum](https://leetcode.com/problems/partition-equal-subset-sum/#/solutions) subset sum. 转化成[01背包问题](http://love-oriented.com/pack/P01.html)。如何从二维数组优化成1维数组

[338. Counting Bits](https://leetcode.com/problems/counting-bits/#/description) DP, 注意位运算符号的优先级

[516. Longest Palindromic Subsequence](https://leetcode.com/problems/longest-palindromic-subsequence/#/description) DP, 求最长回文子序列。
>> 必练题目		
>> 查看solution中从暴力到动态规划的[详细解释](https://leetcode.com/problems/longest-palindromic-subsequence/#/solutions)

[5. Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/#/description) DP, 求最长回文字符串。接上题。
>> 必练题目
>> 

[lintcode 77. Longest Common Subsequence](https://www.lintcode.com/en/problem/longest-common-subsequence/) 经典DP题目，可以查看网易的MIT[公开课视频](http://open.163.com/movie/2010/12/L/4/M6UTT5U0I_M6V2U1HL4.html)讲解。

[4. Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/#/description) 分治，注意数组的corner case

[312. Burst Balloons](https://leetcode.com/problems/burst-balloons/#/description) 分治，动态规划。难点在于如何划分出子问题。

[241. Different Ways to Add Parentheses](https://leetcode.com/problems/different-ways-to-add-parentheses/#/description) 分治，字符串的处理



###分治算法题目汇总
1. merge sort 	
	    注意递归和非递归两种写法，查看我的[github](https://github.com/XingxingHuang/Code_Practice/tree/master/sort)中的代码
	
2. quick sort	
		注意多重写法，查看我的[github](https://github.com/XingxingHuang/Code_Practice/tree/master/sort)中代码.	
		双指针，[partition模板](./template/partition.java)
		
3. binary tree相关操作		
		
		树的遍历	
		二叉树深度	
		平衡二叉树		
	
4. 二分法相关问题			
		大多数二分搜素比较容易。需要注意指针的边界情况处理，建议采用[二分法模板](./template/BinarySearch.java)。
		
5. 大数据题目中很多包含分治思想		
		其核心是排序算法。以及HashMap的应用的相关知识。


分治法，[五大常用算法之一](http://www.cnblogs.com/steven_oyj/archive/2010/05/22/1741370.html)。 分而治之！

| No.| Problem |  Note |
|----|---------|------|
| 004 | [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/) |  每日一题[总结](http://t.cn/RaZ7MDX) | 
| 023 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists/) | 优先队列存链表 | 
| 053 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray/) | [lt 41](http://www.lintcode.com/en/problem/maximum-subarray/) | 
| 169 | [Majority Element](https://leetcode.com/problems/majority-element/) | 多种解法，进阶[229](https://leetcode.com/problems/majority-element-ii/#/description)  | 
| 215 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array/) |  练习 | 
| 218 | [The Skyline Problem](https://leetcode.com/problems/the-skyline-problem/) |   | 
| 240 | [Search a 2D Matrix II](https://leetcode.com/problems/search-a-2d-matrix-ii/) | 简单直接  | 
| 241 | [Different Ways to Add Parentheses](https://leetcode.com/problems/different-ways-to-add-parentheses/) | 练习  | 
| 282 | [Expression Add Operators](https://leetcode.com/problems/expression-add-operators/) |   | 
| 312 | [Burst Balloons](https://leetcode.com/problems/burst-balloons/) |   | 
| 315 | [Count of Smaller Numbers After Self](https://leetcode.com/problems/count-of-smaller-numbers-after-self/) |   | 
| 327 | [Count of Range Sum](https://leetcode.com/problems/count-of-range-sum/) |   | 
| 493 | [Reverse Pairs](https://leetcode.com/problems/reverse-pairs/) |   | 
| 514 | [Freedom Trail](https://leetcode.com/problems/freedom-trail/) |   | 

[399. Evaluate Division](https://leetcode.com/problems/evaluate-division/#/description)  转化除法为图相关问题

[310. Minimum Height Trees](https://leetcode.com/problems/minimum-height-trees) 图，双指针，DFS，BFS均可

[207. Course Schedule](https://leetcode.com/problems/course-schedule/#/description)	

[210. Course Schedule II](https://leetcode.com/problems/course-schedule-ii/#/description)

[133. Clone Graph] (https://leetcode.com/problems/clone-graph/#/description) 图，BFS分层遍历, DFS递归遍历。

[491. Increasing Subsequences](https://leetcode.com/problems/increasing-subsequences/#/description) DFS，subset相关

[274. H-Index](https://leetcode.com/problems/h-index/#/description) 排序问题。

[275. H-Index II](https://leetcode.com/problems/h-index-ii/#/description) 二分法

[75. Sort Colors](https://leetcode.com/problems/sort-colors/#/solutions) 一般的partition方法无法解决，需要三个指针。注意！！

[624. Maximum Distance in Arrays](https://leetcode.com/contest/leetcode-weekly-contest-37/problems/maximum-distance-in-arrays/) 

/**
 * 
 * @author  Xingxing Huang	
 * @since   2017.06.17	
 * @Time    O(n) 	
 * @param   
 * @return  
 */
 
 