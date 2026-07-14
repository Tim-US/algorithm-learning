# LeetCode Hot 100：45 天 Python 面试执行手册

> 周期：2026-07-14 至 2026-08-27，共 45 天  
> 每天：08:00-09:30，最多 90 分钟  
> 目标：不做困难题；编码训练 60 道非困难题（30 道主练、30 道伴练），另外 28 道完成题型识别，覆盖 Hot 100 中全部 88 道简单和中等题。

## 1. 每天只按这个顺序执行

普通学习日固定使用以下时间盒，不临时加时。每天进入对应日期后，只能从上到下逐项勾选；上一项没有处理完，也要在规定时间结束后进入下一项：

1. `08:00-08:10`：做当天到期的间隔复习卡，优先顺序为红题、黄题、绿题。
2. `08:10-08:25`：打开当天“知识”链接，只学习指定内容。
3. `08:25-09:05`：主练题，限时 40 分钟，必须在力扣提交。
4. `09:05-09:20`：伴练题，先判断题型；到达当阶段的提示阈值后仍无思路，就看题解并复现核心代码。
5. `09:20-09:25`：第 1-28 天打开当天的非困难地图题，只读题并判断题型；第 29-35 天改为口述一张到期复习卡。
6. `09:25-09:30`：记录错因、复杂度，并给当天主练题建立复习卡。

每道主练题固定在完成后的第 `1、3、7、14` 天做提取练习。每张卡最多 2 分钟，只回答四件事：题型识别信号、核心不变量或状态、复杂度、一个边界用例。各日列出的 `08:00` 复写任务是优先项，剩余时间继续处理当天到期卡；伴练题不进入间隔队列，除非它被标红。

周日是恢复日，统一缩短为 `08:00-09:00`：10 分钟复习、25 分钟主练、15 分钟伴练、5 分钟地图题或复习卡、5 分钟记录。到点停止，不补时。

主练题不是要求硬想 40 分钟。使用下面的卡题协议：

- 读题和手算样例最多 5 分钟。
- 第 1-7 天独立寻找思路最多 10 分钟，然后允许看范例讲解；第 8-28 天为 15 分钟；第 29-35 天为 20 分钟；第 36-45 天模拟阶段禁止提示。
- 没有方向时，只看当天给出的题解，不继续耗时间。
- 看完题解后关闭页面，从空白编辑器重新写。
- 当天仍写不出就标记为红色，不挤占第二天的新题时间，留到周六处理。

完成状态使用下面四种标记；“掌握数量”只统计绿题：

- `首通`：同一天不看提示完成。这只能说明即时表现，暂不算掌握。
- `绿`：至少间隔 3 天后，不看提示在 25 分钟内完成，并能讲复杂度和边界。
- `黄`：看提示或出现实现错误，但能关掉题解复现。
- `红`：看完题解仍无法独立复现。

开始第 1 天前先做 10 分钟 Python 门槛检查：不查资料写出一个函数、一次 `for + enumerate`、一次 `dict.get` 计数、一次 `list.append/pop`。四项中少于三项成功时，第 1-3 天暂停伴练题，把伴练时间改为 [Python 数据结构教程](https://docs.python.org/zh-cn/3/tutorial/datastructures.html)练习；不补双倍任务。

每次周测后使用同一负荷门槛：至少一题达到绿或首通、另一题不低于黄，才保持下一周两题结构。两题都红时，下一周所有伴练时段改为旧主练题复现，直到连续两次延迟复测成功。该规则优先于日程表。

困难题不进入本计划。力扣标记为“困难”的题即使出现在 Hot 100 页面，也不要打开、不要做、不要补；节省下来的时间全部用于复习简单和中等题。

## 2. 固定入口

- [力扣 Hot 100 总题单](https://leetcode.cn/studyplan/top-100-liked/)
- [《Hello 算法》在线版](https://www.hello-algo.com/)
- [《Hello 算法》简体中文 Python PDF](https://github.com/krahets/hello-algo/releases/download/1.3.0/hello-algo_1.3.0_zh_python.pdf)
- [《Hello 算法》GitHub 中文原文](https://github.com/krahets/hello-algo/tree/main/docs)：在线版打不开时使用
- [代码随想录](https://programmercarl.com/)
- [Python 官方教程：数据结构](https://docs.python.org/zh-cn/3/tutorial/datastructures.html)

不要同时搜索多个题解。当天提供了代码随想录链接时优先看它；没有时进入力扣题解页，选择一篇 Python 高赞题解。

### 第 1-28 天：每天 5 分钟非困难地图题

这 28 题不计入“会做”，只用来补齐非困难题认知。当天只完成三步：读题、说出最可能的题型、记录一句“我为什么这样判断”。禁止编码和看题解。第 28 天结束后，Hot 100 中 88 道非困难题才算全部见过。

| 天数 | 地图题 | 天数 | 地图题 |
|---:|---|---:|---|
| 1 | [LC 128 最长连续序列](https://leetcode.cn/problems/longest-consecutive-sequence/) | 15 | [LC 153 寻找旋转排序数组中的最小值](https://leetcode.cn/problems/find-minimum-in-rotated-sorted-array/) |
| 2 | [LC 189 轮转数组](https://leetcode.cn/problems/rotate-array/) | 16 | [LC 394 字符串解码](https://leetcode.cn/problems/decode-string/) |
| 3 | [LC 73 矩阵置零](https://leetcode.cn/problems/set-matrix-zeroes/) | 17 | [LC 45 跳跃游戏 II](https://leetcode.cn/problems/jump-game-ii/) |
| 4 | [LC 54 螺旋矩阵](https://leetcode.cn/problems/spiral-matrix/) | 18 | [LC 763 划分字母区间](https://leetcode.cn/problems/partition-labels/) |
| 5 | [LC 48 旋转图像](https://leetcode.cn/problems/rotate-image/) | 19 | [LC 118 杨辉三角](https://leetcode.cn/problems/pascals-triangle/) |
| 6 | [LC 240 搜索二维矩阵 II](https://leetcode.cn/problems/search-a-2d-matrix-ii/) | 20 | [LC 279 完全平方数](https://leetcode.cn/problems/perfect-squares/) |
| 7 | [LC 138 随机链表的复制](https://leetcode.cn/problems/copy-list-with-random-pointer/) | 21 | [LC 152 乘积最大子数组](https://leetcode.cn/problems/maximum-product-subarray/) |
| 8 | [LC 146 LRU 缓存](https://leetcode.cn/problems/lru-cache/) | 22 | [LC 416 分割等和子集](https://leetcode.cn/problems/partition-equal-subset-sum/) |
| 9 | [LC 114 二叉树展开为链表](https://leetcode.cn/problems/flatten-binary-tree-to-linked-list/) | 23 | [LC 64 最小路径和](https://leetcode.cn/problems/minimum-path-sum/) |
| 10 | [LC 105 前序与中序构造二叉树](https://leetcode.cn/problems/construct-binary-tree-from-preorder-and-inorder-traversal/) | 24 | [LC 5 最长回文子串](https://leetcode.cn/problems/longest-palindromic-substring/) |
| 11 | [LC 437 路径总和 III](https://leetcode.cn/problems/path-sum-iii/) | 25 | [LC 72 编辑距离](https://leetcode.cn/problems/edit-distance/) |
| 12 | [LC 17 电话号码的字母组合](https://leetcode.cn/problems/letter-combinations-of-a-phone-number/) | 26 | [LC 75 颜色分类](https://leetcode.cn/problems/sort-colors/) |
| 13 | [LC 131 分割回文串](https://leetcode.cn/problems/palindrome-partitioning/) | 27 | [LC 31 下一个排列](https://leetcode.cn/problems/next-permutation/) |
| 14 | [LC 34 查找第一个和最后一个位置](https://leetcode.cn/problems/find-first-and-last-position-of-element-in-sorted-array/) | 28 | [LC 287 寻找重复数](https://leetcode.cn/problems/find-the-duplicate-number/) |

## 3. 第一阶段：数组、哈希、双指针和窗口

### 第 1 天｜7 月 14 日，周二｜哈希表入门

> 今日概览：学习哈希表和字典，用键值映射解决查找与分组问题，建立“用空间换时间”的意识。

- [ ] `08:00-08:10` 完成 Python 门槛检查：函数、`for + enumerate`、`dict.get` 计数、`list.append/pop`；少于三项成功就按总则暂停第 1-3 天的伴练，并使用 [Python 数据结构教程](https://docs.python.org/zh-cn/3/tutorial/datastructures.html)。
- [ ] `08:10-08:25` 阅读《Hello 算法》[哈希表](https://github.com/krahets/hello-algo/blob/main/docs/chapter_hashing/hash_map.md)，只掌握“键值对、查询平均 O(1)、空间换时间”。
- [ ] 主练：[LC 1 两数之和](https://leetcode.cn/problems/two-sum/)；卡住后看[代码随想录题解](https://programmercarl.com/0001.两数之和.html)。
- [ ] 伴练：[LC 49 字母异位词分组](https://leetcode.cn/problems/group-anagrams/)；卡住后看[代码随想录 Hot 100 题解](https://programmercarl.com/hot100/0049.group-anagrams.html)。
- [ ] 地图题：[LC 128 最长连续序列](https://leetcode.cn/problems/longest-consecutive-sequence/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：能解释为什么补数应在查询之后或之前写入，以及如何用排序后的字符串或字符计数作键。

### 第 2 天｜7 月 15 日，周三｜数组原地修改与前后缀

> 今日概览：学习数组原地操作与前后缀积，理解双指针和两次扫描中每个变量的含义。

- [ ] `08:00-08:10` 空白写出第 1 天的 `seen = {}` 主循环。
- [ ] `08:10-08:25` 阅读《Hello 算法》[数组](https://github.com/krahets/hello-algo/blob/main/docs/chapter_array_and_linkedlist/array.md)，只看访问、插入删除和遍历复杂度。
- [ ] 主练：[LC 283 移动零](https://leetcode.cn/problems/move-zeroes/)；卡住后看[代码随想录题解](https://programmercarl.com/0283.移动零.html)。
- [ ] 伴练：[LC 238 除自身以外数组的乘积](https://leetcode.cn/problems/product-of-array-except-self/)；卡住后看[力扣题解](https://leetcode.cn/problems/product-of-array-except-self/solutions/)。
- [ ] 地图题：[LC 189 轮转数组](https://leetcode.cn/problems/rotate-array/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：移动零做到 O(n) 且不复制数组；乘积题能说清 `answer[i]` 在两次扫描中的含义。

### 第 3 天｜7 月 16 日，周四｜相向双指针

> 今日概览：学习相向双指针，通过移动较弱一侧缩小范围，并掌握三数之和的去重方法。

- [ ] `08:00-08:10` 复写移动零的快慢指针更新顺序。
- [ ] `08:10-08:25` 阅读[代码随想录：三数之和](https://programmercarl.com/0015.三数之和.html)中的“思路”和“去重逻辑”，暂时不要抄代码。
- [ ] 主练：[LC 11 盛最多水的容器](https://leetcode.cn/problems/container-with-most-water/)；卡住后看[代码随想录 Hot 100 题解](https://programmercarl.com/hot100/0011.container-with-most-water.html)。
- [ ] 伴练：[LC 15 三数之和](https://leetcode.cn/problems/3sum/)；题解使用上面的代码随想录页面。
- [ ] 地图题：[LC 73 矩阵置零](https://leetcode.cn/problems/set-matrix-zeroes/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：能证明容器题为什么移动短板；三数之和能区分“答案去重”和“指针移动”。

### 第 4 天｜7 月 17 日，周五｜滑动窗口

> 今日概览：学习滑动窗口，明确右端扩张、左端收缩以及窗口满足条件的判断方法。

- [ ] `08:00-08:10` 口述相向双指针适用条件。
- [ ] `08:10-08:25` 阅读[代码随想录：滑动窗口](https://programmercarl.com/0209.长度最小的子数组.html)，只掌握 `right` 扩张、条件满足时 `left` 收缩。
- [ ] 主练：[LC 3 无重复字符的最长子串](https://leetcode.cn/problems/longest-substring-without-repeating-characters/)；卡住后看[代码随想录 Hot 100 题解](https://programmercarl.com/hot100/0003.longest-substring-without-repeating-characters.html)。
- [ ] 伴练：[LC 438 找到字符串中所有字母异位词](https://leetcode.cn/problems/find-all-anagrams-in-a-string/)；卡住后看[力扣题解](https://leetcode.cn/problems/find-all-anagrams-in-a-string/solutions/)。
- [ ] 地图题：[LC 54 螺旋矩阵](https://leetcode.cn/problems/spiral-matrix/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：写出窗口不变量；不能只背 `while`，要能解释窗口什么时候合法。

### 第 5 天｜7 月 18 日，周六｜第一次周测

> 今日概览：闭卷复写本周两道代表题，检查哈希表与滑动窗口是否真正记住。

- [ ] `08:00-08:35` 关闭题解，重做 [LC 1 两数之和](https://leetcode.cn/problems/two-sum/)，写完后讲时间和空间复杂度。
- [ ] `08:35-09:15` 关闭题解，重做 [LC 3 无重复字符的最长子串](https://leetcode.cn/problems/longest-substring-without-repeating-characters/)。
- [ ] `09:15-09:20` 地图题：[LC 48 旋转图像](https://leetcode.cn/problems/rotate-image/)；只读题并判断题型。
- [ ] `09:20-09:30` 对照第 1 天和第 4 天的题解，只记录差异。

### 第 6 天｜7 月 19 日，周日｜轻量位运算与投票

> 今日概览：用较轻负荷学习异或和多数投票法，完成核心任务后按时结束。

- [ ] `08:00-08:10` 复习本周错题，不学习新理论。
- [ ] `08:10-08:35` 主练：[LC 136 只出现一次的数字](https://leetcode.cn/problems/single-number/)；卡住后看[力扣题解](https://leetcode.cn/problems/single-number/solutions/)，只学习异或的三个性质。
- [ ] `08:35-08:50` 伴练：[LC 169 多数元素](https://leetcode.cn/problems/majority-element/)；卡住后看[力扣题解](https://leetcode.cn/problems/majority-element/solutions/)，优先理解 Boyer-Moore 投票法。
- [ ] `08:50-08:55` 地图题：[LC 240 搜索二维矩阵 II](https://leetcode.cn/problems/search-a-2d-matrix-ii/)；只读题并判断题型。
- [ ] `08:55-09:00` 记录后停止。

### 第 7 天｜7 月 20 日，周一｜前缀和与最大连续子数组

> 今日概览：学习前缀和计数与最大连续子数组，重点理解查询和更新的先后顺序。

- [ ] `08:00-08:10` 写出“前缀和之差表示一段区间和”的公式。
- [ ] `08:10-08:25` 阅读[代码随想录：和为 K 的子数组](https://programmercarl.com/hot100/0560.subarray-sum-equals-k.html)中的前缀和定义。
- [ ] 主练：[LC 560 和为 K 的子数组](https://leetcode.cn/problems/subarray-sum-equals-k/)；题解使用上面的代码随想录页面。
- [ ] 伴练：[LC 53 最大子数组和](https://leetcode.cn/problems/maximum-subarray/)；卡住后看[代码随想录题解](https://programmercarl.com/0053.最大子序和.html)。
- [ ] 地图题：[LC 138 随机链表的复制](https://leetcode.cn/problems/copy-list-with-random-pointer/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：能解释为什么前缀计数字典初始为 `{0: 1}`；能说出 `current_sum` 的状态定义。

## 4. 第二阶段：链表、栈和二分

### 第 8 天｜7 月 21 日，周二｜链表指针基础

> 今日概览：进入链表，学习指针重连与相交判断，重点防止修改指针时丢失后继节点。

- [ ] `08:00-08:10` 复写第 7 天的前缀和字典更新顺序。
- [ ] `08:10-08:25` 阅读[代码随想录：链表理论基础](https://programmercarl.com/链表理论基础.html)，只看节点结构、遍历和增删复杂度。
- [ ] 主练：[LC 206 反转链表](https://leetcode.cn/problems/reverse-linked-list/)；卡住后看[代码随想录题解](https://programmercarl.com/0206.翻转链表.html)。
- [ ] 伴练：[LC 160 相交链表](https://leetcode.cn/problems/intersection-of-two-linked-lists/)；卡住后看[代码随想录题解](https://programmercarl.com/0160.相交链表.html)。
- [ ] 地图题：[LC 146 LRU 缓存](https://leetcode.cn/problems/lru-cache/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：反转时能解释 `prev/current/next`；相交比较节点身份而不是节点值。

### 第 9 天｜7 月 22 日，周三｜快慢指针

> 今日概览：学习快慢指针处理回文和环，弄清奇偶长度下两个指针的停止位置。

- [ ] `08:00-08:10` 从空白写出迭代反转链表。
- [ ] `08:10-08:25` 阅读[代码随想录：环形链表 II](https://programmercarl.com/0142.环形链表II.html)中快慢指针相遇的图解。
- [ ] 主练：[LC 234 回文链表](https://leetcode.cn/problems/palindrome-linked-list/)；卡住后看[代码随想录题解](https://programmercarl.com/0234.回文链表.html)。
- [ ] 伴练：[LC 141 环形链表](https://leetcode.cn/problems/linked-list-cycle/)；卡住后看[代码随想录题解](https://programmercarl.com/0141.环形链表.html)。
- [ ] 地图题：[LC 114 二叉树展开为链表](https://leetcode.cn/problems/flatten-binary-tree-to-linked-list/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：能找到链表中点，并能说明奇偶长度下快慢指针停止位置。

### 第 10 天｜7 月 23 日，周四｜环入口与链表合并

> 今日概览：学习寻找环入口和合并有序链表，开始熟练使用虚拟头节点。

- [ ] `08:00-08:10` 口述快慢指针为什么一定会在环内相遇。
- [ ] `08:10-08:25` 继续阅读[环形链表 II](https://programmercarl.com/0142.环形链表II.html)的入口推导，只需记住相遇后一个指针回到头节点。
- [ ] 主练：[LC 142 环形链表 II](https://leetcode.cn/problems/linked-list-cycle-ii/)；题解使用上面的代码随想录页面。
- [ ] 伴练：[LC 21 合并两个有序链表](https://leetcode.cn/problems/merge-two-sorted-lists/)；卡住后看[力扣题解](https://leetcode.cn/problems/merge-two-sorted-lists/solutions/)。
- [ ] 地图题：[LC 105 前序与中序构造二叉树](https://leetcode.cn/problems/construct-binary-tree-from-preorder-and-inorder-traversal/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：会使用虚拟头节点 `dummy`，返回 `dummy.next`。

### 第 11 天｜7 月 24 日，周五｜虚拟头节点与间距指针

> 今日概览：学习链表进位和固定间距双指针，统一处理删除头节点等边界情况。

- [ ] `08:00-08:10` 复写合并链表的 `dummy/tail` 初始化。
- [ ] `08:10-08:25` 阅读[代码随想录：删除倒数第 N 个节点](https://programmercarl.com/0019.删除链表的倒数第N个节点.html)，重点看双指针间距。
- [ ] 主练：[LC 2 两数相加](https://leetcode.cn/problems/add-two-numbers/)；卡住后看[力扣题解](https://leetcode.cn/problems/add-two-numbers/solutions/)。
- [ ] 伴练：[LC 19 删除链表的倒数第 N 个节点](https://leetcode.cn/problems/remove-nth-node-from-end-of-list/)；题解使用上面的代码随想录页面。
- [ ] 地图题：[LC 437 路径总和 III](https://leetcode.cn/problems/path-sum-iii/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：两数相加不漏最后一个进位；删除头节点时无需特殊分支。

### 第 12 天｜7 月 25 日，周六｜链表周测

> 今日概览：闭卷复写反转链表和删除倒数节点，检查指针操作是否稳定。

- [ ] `08:00-08:35` 限时重做 [LC 206 反转链表](https://leetcode.cn/problems/reverse-linked-list/)，再用 `[1, 2]` 手动走一遍。
- [ ] `08:35-09:15` 限时重做 [LC 19 删除倒数第 N 个节点](https://leetcode.cn/problems/remove-nth-node-from-end-of-list/)。
- [ ] `09:15-09:20` 地图题：[LC 17 电话号码的字母组合](https://leetcode.cn/problems/letter-combinations-of-a-phone-number/)；只读题并判断题型。
- [ ] `09:20-09:30` 画出指针变化并记录错误。

### 第 13 天｜7 月 26 日，周日｜栈与二分入门

> 今日概览：轻量学习栈与二分查找，重点保持搜索区间的定义前后一致。

- [ ] `08:00-08:10` 阅读[栈与队列理论基础](https://programmercarl.com/栈与队列理论基础.html)和《Hello 算法》[二分查找](https://github.com/krahets/hello-algo/blob/main/docs/chapter_searching/binary_search.md)，只看核心定义。
- [ ] `08:10-08:35` 主练：[LC 20 有效的括号](https://leetcode.cn/problems/valid-parentheses/)；卡住后看[代码随想录题解](https://programmercarl.com/0020.有效的括号.html)。
- [ ] `08:35-08:50` 伴练：[LC 35 搜索插入位置](https://leetcode.cn/problems/search-insert-position/)；卡住后看[代码随想录题解](https://programmercarl.com/0035.搜索插入位置.html)。
- [ ] `08:50-08:55` 地图题：[LC 131 分割回文串](https://leetcode.cn/problems/palindrome-partitioning/)；只读题并判断题型。
- [ ] `08:55-09:00` 记录二分区间定义后停止。

### 第 14 天｜7 月 27 日，周一｜链表递归与归并

> 今日概览：学习链表递归和归并排序，掌握“分开、处理、合并”的整体思路。

- [ ] `08:00-08:10` 写出栈匹配括号使用的映射表。
- [ ] `08:10-08:25` 阅读《Hello 算法》[归并排序](https://github.com/krahets/hello-algo/blob/main/docs/chapter_sorting/merge_sort.md)，只看“分开、排序、合并”三个步骤。
- [ ] 主练：[LC 24 两两交换链表中的节点](https://leetcode.cn/problems/swap-nodes-in-pairs/)；卡住后看[代码随想录题解](https://programmercarl.com/0024.两两交换链表中的节点.html)。
- [ ] 伴练：[LC 148 排序链表](https://leetcode.cn/problems/sort-list/)；卡住后看[力扣题解](https://leetcode.cn/problems/sort-list/solutions/)，只要求理解归并方案。
- [ ] 地图题：[LC 34 查找第一个和最后一个位置](https://leetcode.cn/problems/find-first-and-last-position-of-element-in-sorted-array/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：能说明排序链表为什么需要快慢指针找中点，以及合并两个有序链表如何复用。

## 5. 第三阶段：二叉树

### 第 15 天｜7 月 28 日，周二｜树与递归遍历

> 今日概览：学习二叉树节点、递归遍历与深度计算，明确递归函数应该返回什么。

- [ ] `08:00-08:10` 口述递归函数的参数、返回值和终止条件。
- [ ] `08:10-08:25` 阅读[二叉树理论基础](https://programmercarl.com/二叉树理论基础.html)和[二叉树递归遍历](https://programmercarl.com/二叉树的递归遍历.html)，只看 Python 递归框架。
- [ ] 主练：[LC 94 二叉树的中序遍历](https://leetcode.cn/problems/binary-tree-inorder-traversal/)；卡住后看[力扣题解](https://leetcode.cn/problems/binary-tree-inorder-traversal/solutions/)。
- [ ] 伴练：[LC 104 二叉树的最大深度](https://leetcode.cn/problems/maximum-depth-of-binary-tree/)；卡住后看[代码随想录题解](https://programmercarl.com/0104.二叉树的最大深度.html)。
- [ ] 地图题：[LC 153 寻找旋转排序数组中的最小值](https://leetcode.cn/problems/find-minimum-in-rotated-sorted-array/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：能区分“遍历过程维护答案”和“递归返回子问题答案”。

### 第 16 天｜7 月 29 日，周三｜左右子树递归

> 今日概览：练习左右子树递归，掌握翻转和镜像比较中的对应关系。

- [ ] `08:00-08:10` 默写最大深度的递归终止条件。
- [ ] `08:10-08:25` 复读[二叉树递归遍历](https://programmercarl.com/二叉树的递归遍历.html)，把前、中、后序各写成一行顺序。
- [ ] 主练：[LC 226 翻转二叉树](https://leetcode.cn/problems/invert-binary-tree/)；卡住后看[代码随想录题解](https://programmercarl.com/0226.翻转二叉树.html)。
- [ ] 伴练：[LC 101 对称二叉树](https://leetcode.cn/problems/symmetric-tree/)；卡住后看[代码随想录题解](https://programmercarl.com/0101.对称二叉树.html)。
- [ ] 地图题：[LC 394 字符串解码](https://leetcode.cn/problems/decode-string/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：对称树比较的是“外侧与外侧、内侧与内侧”。

### 第 17 天｜7 月 30 日，周四｜后序信息与层序遍历

> 今日概览：学习后序返回信息和层序遍历，区分递归与队列的使用场景。

- [ ] `08:00-08:10` 复写翻转二叉树，禁止看昨天代码。
- [ ] `08:10-08:25` 阅读《Hello 算法》[二叉树遍历](https://github.com/krahets/hello-algo/blob/main/docs/chapter_tree/binary_tree_traversal.md)，重点看层序遍历使用队列。
- [ ] 主练：[LC 543 二叉树的直径](https://leetcode.cn/problems/diameter-of-binary-tree/)；卡住后看[力扣题解](https://leetcode.cn/problems/diameter-of-binary-tree/solutions/)。
- [ ] 伴练：[LC 102 二叉树的层序遍历](https://leetcode.cn/problems/binary-tree-level-order-traversal/)；卡住后看[代码随想录题解](https://programmercarl.com/0102.二叉树的层序遍历.html)。
- [ ] 地图题：[LC 45 跳跃游戏 II](https://leetcode.cn/problems/jump-game-ii/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：直径用左右深度之和更新全局答案；层序遍历进入每层前固定队列长度。

### 第 18 天｜7 月 31 日，周五｜二叉搜索树

> 今日概览：学习二叉搜索树的有序性质，用中序遍历完成验证和计数。

- [ ] `08:00-08:10` 写出层序遍历的 `for _ in range(len(queue))` 框架。
- [ ] `08:10-08:25` 阅读《Hello 算法》[二叉搜索树](https://github.com/krahets/hello-algo/blob/main/docs/chapter_tree/binary_search_tree.md)，只掌握有序性质和中序遍历结果递增。
- [ ] 主练：[LC 98 验证二叉搜索树](https://leetcode.cn/problems/validate-binary-search-tree/)；卡住后看[代码随想录题解](https://programmercarl.com/0098.验证二叉搜索树.html)。
- [ ] 伴练：[LC 230 二叉搜索树中第 K 小的元素](https://leetcode.cn/problems/kth-smallest-element-in-a-bst/)；卡住后看[力扣题解](https://leetcode.cn/problems/kth-smallest-element-in-a-bst/solutions/)。
- [ ] 地图题：[LC 763 划分字母区间](https://leetcode.cn/problems/partition-labels/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：不能只比较父子节点；要使用上下界或完整中序序列。

### 第 19 天｜8 月 1 日，周六｜二叉树周测

> 今日概览：闭卷复写树的直径与二叉搜索树验证，重点检查递归返回值。

- [ ] `08:00-08:40` 限时重做 [LC 543 二叉树的直径](https://leetcode.cn/problems/diameter-of-binary-tree/)，同时讲清递归函数返回什么。
- [ ] `08:40-09:20` 限时重做 [LC 98 验证二叉搜索树](https://leetcode.cn/problems/validate-binary-search-tree/)。
- [ ] `09:20-09:25` 地图题：[LC 118 杨辉三角](https://leetcode.cn/problems/pascals-triangle/)；只读题并判断题型。
- [ ] `09:25-09:30` 记录最容易混淆的递归返回值。

### 第 20 天｜8 月 2 日，周日｜递归构造与动态规划初见

> 今日概览：轻量接触分治和动态规划，用构造平衡树与爬楼梯理解子问题。

- [ ] `08:00-08:10` 阅读《Hello 算法》[分治](https://github.com/krahets/hello-algo/blob/main/docs/chapter_divide_and_conquer/divide_and_conquer.md)和[动态规划简介](https://github.com/krahets/hello-algo/blob/main/docs/chapter_dynamic_programming/intro_to_dynamic_programming.md)的定义。
- [ ] `08:10-08:35` 主练：[LC 108 将有序数组转换为二叉搜索树](https://leetcode.cn/problems/convert-sorted-array-to-binary-search-tree/)；卡住后看[代码随想录题解](https://programmercarl.com/0108.将有序数组转换为二叉搜索树.html)。
- [ ] `08:35-08:50` 伴练：[LC 70 爬楼梯](https://leetcode.cn/problems/climbing-stairs/)；卡住后看[代码随想录题解](https://programmercarl.com/0070.爬楼梯.html)。
- [ ] `08:50-08:55` 地图题：[LC 279 完全平方数](https://leetcode.cn/problems/perfect-squares/)；只读题并判断题型。
- [ ] `08:55-09:00` 记录 `dp[i]` 的定义后停止。

### 第 21 天｜8 月 3 日，周一｜树的视图与公共祖先

> 今日概览：学习层序视图与最近公共祖先，重点理解递归返回结果的含义。

- [ ] `08:00-08:10` 复写层序遍历，并指出每层最后一个节点的位置。
- [ ] `08:10-08:25` 阅读[代码随想录：最近公共祖先](https://programmercarl.com/0236.二叉树的最近公共祖先.html)的递归返回值说明，暂不抄代码。
- [ ] 主练：[LC 199 二叉树的右视图](https://leetcode.cn/problems/binary-tree-right-side-view/)；卡住后看[力扣题解](https://leetcode.cn/problems/binary-tree-right-side-view/solutions/)。
- [ ] 伴练：[LC 236 二叉树的最近公共祖先](https://leetcode.cn/problems/lowest-common-ancestor-of-a-binary-tree/)；题解使用上面的代码随想录页面。
- [ ] 地图题：[LC 152 乘积最大子数组](https://leetcode.cn/problems/maximum-product-subarray/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：最近公共祖先函数返回“当前子树找到的 p、q 或其祖先”。

## 6. 第四阶段：图、回溯、二分和栈

### 第 22 天｜8 月 4 日，周二｜网格搜索

> 今日概览：学习网格中的深度和广度优先搜索，正确处理边界与访问标记。

- [ ] `08:00-08:10` 写出深度优先搜索的终止条件模板。
- [ ] `08:10-08:25` 阅读《Hello 算法》[图遍历](https://github.com/krahets/hello-algo/blob/main/docs/chapter_graph/graph_traversal.md)，只比较深度优先搜索使用递归或栈、广度优先搜索使用队列。
- [ ] 主练：[LC 200 岛屿数量](https://leetcode.cn/problems/number-of-islands/)；卡住后看[代码随想录深度优先题解](https://programmercarl.com/0200.岛屿数量.深搜版.html)。
- [ ] 伴练：[LC 994 腐烂的橘子](https://leetcode.cn/problems/rotting-oranges/)；卡住后看[力扣题解](https://leetcode.cn/problems/rotting-oranges/solutions/)。
- [ ] 地图题：[LC 416 分割等和子集](https://leetcode.cn/problems/partition-equal-subset-sum/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：访问后立即标记；腐烂橘子使用多源广度优先搜索，初始腐烂橘子全部入队。

### 第 23 天｜8 月 5 日，周三｜拓扑排序与前缀树

> 今日概览：学习邻接表、入度和前缀树，理解拓扑排序与树形字符存储。

- [ ] `08:00-08:10` 复写网格四方向数组与边界判断。
- [ ] `08:10-08:25` 阅读《Hello 算法》[图的表示与操作](https://github.com/krahets/hello-algo/blob/main/docs/chapter_graph/graph_operations.md)，重点看邻接表；再浏览题解中的入度概念。
- [ ] 主练：[LC 207 课程表](https://leetcode.cn/problems/course-schedule/)；卡住后看[代码随想录题解](https://programmercarl.com/0207.课程表.html)。
- [ ] 伴练：[LC 208 实现前缀树](https://leetcode.cn/problems/implement-trie-prefix-tree/)；卡住后看[力扣题解](https://leetcode.cn/problems/implement-trie-prefix-tree/solutions/)。
- [ ] 地图题：[LC 64 最小路径和](https://leetcode.cn/problems/minimum-path-sum/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：课程表能说出“入度为 0 入队”；前缀树节点包含子节点映射和单词结束标志。

### 第 24 天｜8 月 6 日，周四｜回溯框架

> 今日概览：学习回溯基本框架，按“选择、递归、撤销”生成排列和子集。

- [ ] `08:00-08:10` 说明深度优先搜索与回溯的关系。
- [ ] `08:10-08:25` 阅读[代码随想录：回溯算法理论基础](https://programmercarl.com/回溯算法理论基础.html)，只记住选择、递归、撤销选择。
- [ ] 主练：[LC 46 全排列](https://leetcode.cn/problems/permutations/)；卡住后看[代码随想录题解](https://programmercarl.com/0046.全排列.html)。
- [ ] 伴练：[LC 78 子集](https://leetcode.cn/problems/subsets/)；卡住后看[代码随想录题解](https://programmercarl.com/0078.子集.html)。
- [ ] 地图题：[LC 5 最长回文子串](https://leetcode.cn/problems/longest-palindromic-substring/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：添加答案时使用 `path.copy()`；全排列使用 `used`，子集每个节点都收集答案。

### 第 25 天｜8 月 7 日，周五｜回溯剪枝

> 今日概览：学习回溯剪枝，处理元素复用和括号合法性，避免无效搜索。

- [ ] `08:00-08:10` 空白写出 `backtrack(path, choices)` 骨架。
- [ ] `08:10-08:25` 阅读《Hello 算法》[回溯算法](https://github.com/krahets/hello-algo/blob/main/docs/chapter_backtracking/backtracking_algorithm.md)，只看尝试、回退和剪枝。
- [ ] 主练：[LC 39 组合总和](https://leetcode.cn/problems/combination-sum/)；卡住后看[代码随想录题解](https://programmercarl.com/0039.组合总和.html)。
- [ ] 伴练：[LC 22 括号生成](https://leetcode.cn/problems/generate-parentheses/)；卡住后看[力扣题解](https://leetcode.cn/problems/generate-parentheses/solutions/)。
- [ ] 地图题：[LC 72 编辑距离](https://leetcode.cn/problems/edit-distance/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：组合总和允许复用当前元素；括号生成始终满足右括号数不超过左括号数。

### 第 26 天｜8 月 8 日，周六｜图与回溯周测

> 今日概览：闭卷复写岛屿数量和子集，检查访问标记、结果复制与撤销操作。

- [ ] `08:00-08:40` 限时重做 [LC 200 岛屿数量](https://leetcode.cn/problems/number-of-islands/)。
- [ ] `08:40-09:20` 限时重做 [LC 78 子集](https://leetcode.cn/problems/subsets/)。
- [ ] `09:20-09:25` 地图题：[LC 75 颜色分类](https://leetcode.cn/problems/sort-colors/)；只读题并判断题型。
- [ ] `09:25-09:30` 检查访问标记、撤销选择和 `path.copy()`。

### 第 27 天｜8 月 9 日，周日｜二维二分与辅助栈

> 今日概览：轻量练习二维二分和辅助栈，保持索引映射正确并实现常数时间操作。

- [ ] `08:00-08:10` 复习《Hello 算法》[二分查找](https://github.com/krahets/hello-algo/blob/main/docs/chapter_searching/binary_search.md)和[栈](https://github.com/krahets/hello-algo/blob/main/docs/chapter_stack_and_queue/stack.md)的模板。
- [ ] `08:10-08:35` 主练：[LC 74 搜索二维矩阵](https://leetcode.cn/problems/search-a-2d-matrix/)；卡住后看[力扣题解](https://leetcode.cn/problems/search-a-2d-matrix/solutions/)。
- [ ] `08:35-08:50` 伴练：[LC 155 最小栈](https://leetcode.cn/problems/min-stack/)；卡住后看[力扣题解](https://leetcode.cn/problems/min-stack/solutions/)。
- [ ] `08:50-08:55` 地图题：[LC 31 下一个排列](https://leetcode.cn/problems/next-permutation/)；只读题并判断题型。
- [ ] `08:55-09:00` 记录后停止。

### 第 28 天｜8 月 10 日，周一｜网格回溯与旋转数组二分

> 今日概览：结合网格回溯与旋转数组二分，练习恢复现场和判断有序区间。

- [ ] `08:00-08:10` 复写二分闭区间模板。
- [ ] `08:10-08:25` 阅读《Hello 算法》[回溯：全排列问题](https://github.com/krahets/hello-algo/blob/main/docs/chapter_backtracking/permutations_problem.md)中“状态和选择”的表述。
- [ ] 主练：[LC 79 单词搜索](https://leetcode.cn/problems/word-search/)；卡住后看[力扣题解](https://leetcode.cn/problems/word-search/solutions/)。
- [ ] 伴练：[LC 33 搜索旋转排序数组](https://leetcode.cn/problems/search-in-rotated-sorted-array/)；卡住后看[力扣题解](https://leetcode.cn/problems/search-in-rotated-sorted-array/solutions/)。
- [ ] 地图题：[LC 287 寻找重复数](https://leetcode.cn/problems/find-the-duplicate-number/)；只读题并说出可能题型，不编码、不看题解。
- [ ] 验收：单词搜索退出递归前恢复现场；旋转数组每轮先判断哪一半有序。

## 7. 第五阶段：栈、堆、贪心和动态规划

### 第 29 天｜8 月 11 日，周二｜单调栈与堆

> 今日概览：学习单调栈与堆，掌握索引存储和维护前 K 个元素的方法。

- [ ] `08:00-08:10` 写出普通栈的入栈和出栈操作。
- [ ] `08:10-08:25` 阅读《Hello 算法》[堆](https://github.com/krahets/hello-algo/blob/main/docs/chapter_heap/heap.md)，只掌握 Python `heapq` 是小顶堆，以及入堆/出堆 O(log n)。
- [ ] 主练：[LC 739 每日温度](https://leetcode.cn/problems/daily-temperatures/)；卡住后看[代码随想录题解](https://programmercarl.com/0739.每日温度.html)。
- [ ] 伴练：[LC 215 数组中的第 K 个最大元素](https://leetcode.cn/problems/kth-largest-element-in-an-array/)；卡住后看[力扣题解](https://leetcode.cn/problems/kth-largest-element-in-an-array/solutions/)。
- [ ] `09:20-09:25` 复习卡：口述一张当天到期的主练题卡片。
- [ ] 验收：单调栈存索引而非温度；会用大小为 k 的小顶堆维护最大 k 个元素。

### 第 30 天｜8 月 12 日，周三｜前 K 高频与区间排序

> 今日概览：学习频率统计、堆与区间合并，理解排序后依次处理的价值。

- [ ] `08:00-08:10` 写出 `heapq.heappush/heappop` 的最小示例。
- [ ] `08:10-08:25` 阅读《Hello 算法》[前 K 个元素问题](https://github.com/krahets/hello-algo/blob/main/docs/chapter_heap/top_k.md)，再浏览合并区间题解中的排序规则。
- [ ] 主练：[LC 347 前 K 个高频元素](https://leetcode.cn/problems/top-k-frequent-elements/)；卡住后看[代码随想录题解](https://programmercarl.com/0347.前K个高频元素.html)。
- [ ] 伴练：[LC 56 合并区间](https://leetcode.cn/problems/merge-intervals/)；卡住后看[代码随想录题解](https://programmercarl.com/0056.合并区间.html)。
- [ ] `09:20-09:25` 复习卡：口述一张当天到期的主练题卡片。
- [ ] 验收：能解释为什么区间必须先按起点排序，以及何时合并、何时开启新区间。

### 第 31 天｜8 月 13 日，周四｜一维动态规划与完全背包

> 今日概览：学习一维动态规划和完全背包，先定义状态，再写转移和初始化。

- [ ] `08:00-08:10` 写出爬楼梯的状态转移式。
- [ ] `08:10-08:25` 阅读[代码随想录：动态规划理论基础](https://programmercarl.com/动态规划理论基础.html)，只掌握五步：状态、转移、初始化、遍历顺序、打印检查。
- [ ] 主练：[LC 198 打家劫舍](https://leetcode.cn/problems/house-robber/)；卡住后看[代码随想录题解](https://programmercarl.com/0198.打家劫舍.html)。
- [ ] 伴练：[LC 322 零钱兑换](https://leetcode.cn/problems/coin-change/)；卡住后看[代码随想录题解](https://programmercarl.com/0322.零钱兑换.html)。
- [ ] `09:20-09:25` 复习卡：口述一张当天到期的主练题卡片。
- [ ] 验收：先用一句中文定义 `dp[i]`；零钱兑换不可达状态使用无穷大。

### 第 32 天｜8 月 14 日，周五｜背包与序列动态规划

> 今日概览：学习背包与序列动态规划，先掌握清楚可靠的平方时间解法。

- [ ] `08:00-08:10` 复写打家劫舍的两个选择：抢当前或不抢当前。
- [ ] `08:10-08:25` 阅读《Hello 算法》[动态规划解题思路](https://github.com/krahets/hello-algo/blob/main/docs/chapter_dynamic_programming/dp_solution_pipeline.md)，只看状态定义和转移方程。
- [ ] 主练：[LC 139 单词拆分](https://leetcode.cn/problems/word-break/)；卡住后看[代码随想录题解](https://programmercarl.com/0139.单词拆分.html)。
- [ ] 伴练：[LC 300 最长递增子序列](https://leetcode.cn/problems/longest-increasing-subsequence/)；卡住后看[代码随想录题解](https://programmercarl.com/0300.最长上升子序列.html)。
- [ ] `09:20-09:25` 复习卡：口述一张当天到期的主练题卡片。
- [ ] 验收：`dp[i]` 的定义必须包含下标 i 的含义；先掌握最长递增子序列的 O(n²) 写法，不追求二分优化。

### 第 33 天｜8 月 15 日，周六｜栈、堆和动态规划周测

> 今日概览：闭卷复写每日温度和零钱兑换，检查不变量、初始化与遍历顺序。

- [ ] `08:00-08:40` 限时重做 [LC 739 每日温度](https://leetcode.cn/problems/daily-temperatures/)。
- [ ] `08:40-09:20` 限时重做 [LC 322 零钱兑换](https://leetcode.cn/problems/coin-change/)。
- [ ] `09:20-09:25` 口述一张到期复习卡；`09:25-09:30` 检查单调栈不变量和动态规划初始化。

### 第 34 天｜8 月 16 日，周日｜基础贪心

> 今日概览：轻量学习贪心，用最低价格和最远覆盖范围描述局部最优选择。

- [ ] `08:00-08:10` 阅读[贪心算法理论基础](https://programmercarl.com/贪心算法理论基础.html)，只理解“局部最优选择需要可解释”。
- [ ] `08:10-08:35` 主练：[LC 121 买卖股票的最佳时机](https://leetcode.cn/problems/best-time-to-buy-and-sell-stock/)；卡住后看[代码随想录题解](https://programmercarl.com/0121.买卖股票的最佳时机.html)。
- [ ] `08:35-08:50` 伴练：[LC 55 跳跃游戏](https://leetcode.cn/problems/jump-game/)；卡住后看[代码随想录题解](https://programmercarl.com/0055.跳跃游戏.html)。
- [ ] `08:50-08:55` 口述一张到期复习卡；`08:55-09:00` 记录两个贪心变量后停止。

### 第 35 天｜8 月 17 日，周一｜二维动态规划

> 今日概览：学习二维动态规划，画表理解网格路径和两个序列的对应关系。

- [ ] `08:00-08:10` 用一句话定义一维动态规划状态。
- [ ] `08:10-08:25` 复习《Hello 算法》[动态规划解题思路](https://github.com/krahets/hello-algo/blob/main/docs/chapter_dynamic_programming/dp_solution_pipeline.md)，重点看二维状态表。
- [ ] 主练：[LC 62 不同路径](https://leetcode.cn/problems/unique-paths/)；卡住后看[代码随想录题解](https://programmercarl.com/0062.不同路径.html)。
- [ ] 伴练：[LC 1143 最长公共子序列](https://leetcode.cn/problems/longest-common-subsequence/)；卡住后看[代码随想录题解](https://programmercarl.com/1143.最长公共子序列.html)。
- [ ] `09:20-09:25` 复习卡：口述一张当天到期的主练题卡片。
- [ ] 验收：能画出动态规划表格并解释行列含义；相等和不相等时分别从哪里转移。

## 8. 第六阶段：复写与模拟面试

这一阶段不再系统学习新算法。第 40 天和第 44 天各安排一道只见过题面、没有学过解法的陌生题，用来检验知识迁移，而不是背诵原题代码。

### 第 36 天｜8 月 18 日，周二｜哈希与前缀和复写

> 今日概览：复写哈希与前缀和，重点检查默认计数和查询、更新的先后顺序。

- [ ] `08:00-08:35` 限时完成 [LC 1 两数之和](https://leetcode.cn/problems/two-sum/)，边写边解释哈希表保存什么。
- [ ] `08:35-09:15` 限时完成 [LC 560 和为 K 的子数组](https://leetcode.cn/problems/subarray-sum-equals-k/)。
- [ ] `09:15-09:20` 口述一张到期复习卡；`09:20-09:30` 手算 `[1, -1, 0]` 并检查更新顺序。

### 第 37 天｜8 月 19 日，周三｜双指针与窗口复写

> 今日概览：复写双指针与滑动窗口，检查排序去重和窗口不变量。

- [ ] `08:00-08:45` 限时完成 [LC 15 三数之和](https://leetcode.cn/problems/3sum/)。
- [ ] `08:45-09:20` 限时完成 [LC 438 找到所有字母异位词](https://leetcode.cn/problems/find-all-anagrams-in-a-string/)。
- [ ] `09:20-09:25` 口述一张到期复习卡；`09:25-09:30` 记录去重条件和窗口不变量。

### 第 38 天｜8 月 20 日，周四｜链表复写

> 今日概览：复写链表指针题，用画图确认反转和寻找环入口的过程。

- [ ] `08:00-08:35` 限时完成 [LC 206 反转链表](https://leetcode.cn/problems/reverse-linked-list/)，迭代与递归任选其一。
- [ ] `08:35-09:15` 限时完成 [LC 142 环形链表 II](https://leetcode.cn/problems/linked-list-cycle-ii/)。
- [ ] `09:15-09:20` 口述一张到期复习卡；`09:20-09:30` 手画指针变化和有环链表示例。

### 第 39 天｜8 月 21 日，周五｜二叉树复写

> 今日概览：复写树的层序遍历与递归题，清楚说明队列和返回值的含义。

- [ ] `08:00-08:40` 限时完成 [LC 102 二叉树的层序遍历](https://leetcode.cn/problems/binary-tree-level-order-traversal/)。
- [ ] `08:40-09:20` 限时完成 [LC 236 二叉树的最近公共祖先](https://leetcode.cn/problems/lowest-common-ancestor-of-a-binary-tree/)。
- [ ] `09:20-09:25` 口述一张到期复习卡；`09:25-09:30` 说明广度优先搜索的队列规则和最近公共祖先的递归返回值。

### 第 40 天｜8 月 22 日，周六｜第一次完整模拟

> 今日概览：用一道陌生题和一道旧题进行完整模拟，检验知识迁移与表达能力。

- [ ] `08:00-08:05` 像面试一样澄清输入输出，不看历史提交。
- [ ] `08:05-08:40` 独立完成陌生题 [LC 128 最长连续序列](https://leetcode.cn/problems/longest-consecutive-sequence/)，不得查看第 1 天的地图记录。
- [ ] `08:40-09:15` 完成 [LC 56 合并区间](https://leetcode.cn/problems/merge-intervals/)。
- [ ] `09:15-09:30` 复盘题型识别、边界情况、复杂度和表达，不再增加题目。

### 第 41 天｜8 月 23 日，周日｜恢复日

> 今日概览：主动恢复，只整理错题和默写五个框架，不做新题。

- [ ] `08:00-08:20` 只看错题记录，把红题按哈希、双指针、链表、树、图、回溯、动态规划分类。
- [ ] `08:20-08:50` 默写五个骨架：二分、滑动窗口、链表反转、树的深度优先搜索、图的广度优先搜索。
- [ ] `08:50-09:00` 口述面试流程后停止；不提交题目。

### 第 42 天｜8 月 24 日，周一｜图与回溯复写

> 今日概览：复写图和回溯，检查入度更新、剪枝条件与撤销选择。

- [ ] `08:00-08:40` 限时完成 [LC 207 课程表](https://leetcode.cn/problems/course-schedule/)。
- [ ] `08:40-09:20` 限时完成 [LC 39 组合总和](https://leetcode.cn/problems/combination-sum/)。
- [ ] `09:20-09:30` 检查入度更新、剪枝条件和撤销选择。

### 第 43 天｜8 月 25 日，周二｜堆与二维动态规划

> 今日概览：复写堆和二维动态规划，说明数据结构选择和状态表的含义。

- [ ] `08:00-08:35` 限时完成 [LC 215 数组中的第 K 个最大元素](https://leetcode.cn/problems/kth-largest-element-in-an-array/)。
- [ ] `08:35-09:20` 限时完成 [LC 1143 最长公共子序列](https://leetcode.cn/problems/longest-common-subsequence/)。
- [ ] `09:20-09:30` 解释堆的复杂度和二维动态规划表格的含义。

### 第 44 天｜8 月 26 日，周三｜最终模拟

> 今日概览：用陌生栈题和旧回溯题进行模拟，检查独立解题和口头表达能力。

- [ ] `08:00-08:05` 开场澄清题意和约束。
- [ ] `08:05-08:40` 独立完成陌生题 [LC 394 字符串解码](https://leetcode.cn/problems/decode-string/)，不得查看第 16 天的地图记录。
- [ ] `08:40-09:15` 完成 [LC 79 单词搜索](https://leetcode.cn/problems/word-search/)。
- [ ] `09:15-09:30` 完整口述：暴力方案、优化依据、代码、样例、复杂度。

### 第 45 天｜8 月 27 日，周四｜收尾与信心题

> 今日概览：用两道信心题收尾，口述中等题方案，不再接触新知识。

- [ ] `08:00-08:25` 无提示完成 [LC 1 两数之和](https://leetcode.cn/problems/two-sum/)。
- [ ] `08:25-08:55` 无提示完成 [LC 206 反转链表](https://leetcode.cn/problems/reverse-linked-list/)。
- [ ] `08:55-09:15` 口述两个中等题的方案，不再编码：三数之和、二叉树最近公共祖先。
- [ ] `09:15-09:30` 浏览错题表和面试流程，停止学习新内容。

## 9. 每题记录模板

每天在本文件末尾或自己的笔记中追加一条，不要抄完整题解：

```text
日期：
题目：
任务类型：主练 / 伴练 / 地图题
首次状态：首通 / 黄 / 红
延迟状态：绿 / 黄 / 红（至少 3 天后填写）
识别信号：看到什么条件，应想到什么题型？
核心不变量或 dp 定义：
本次错误：
边界用例：
时间复杂度 / 空间复杂度：
主练复习日：完成后的第 1 / 3 / 7 / 14 天
```

## 10. 向 AI 求助时直接使用

第一次卡住：

```text
我正在做 LeetCode <题号和标题>。不要给完整答案，也不要写代码。
请先检查我对题意的理解，然后只给一个能让我继续推进的提示。
```

写完代码后：

```text
请按算法面试标准审查下面的 Python 代码，只指出：
1. 逻辑错误；2. 漏掉的边界情况；3. 时间和空间复杂度；4. Python 实现风险。
先不要给修改后的完整代码。
```

模拟面试：

```text
请对我进行 35 分钟算法模拟面试。一次只扮演面试官，不主动给提示。
要求我先澄清题目、提出暴力解法、优化、编码、手算样例并分析复杂度。
```

## 11. 不掉队规则

- 某天缺席：第二天继续原计划，不补双倍任务；把缺席题移到最近的周六。
- 主练题超时：20 分钟无方向就看题解，学习目标是复现，不是硬耗。
- 伴练题没写完：只要求讲出题型、关键状态和复杂度，不占用第二天。
- 连续两天疲劳：第三天只做 45 分钟复写，不做新题。
- 周测两题都红：下一周减少一道伴练题，优先补基础，不扩大题量。
- 每晚睡眠明显不足时，不用早起硬刷；当天改为任意连续 45 分钟的复写，不做新题。疲劳状态下增加题量不会补回学习效果。

阶段检查点：

- 第 12 天：周测至少一题达到首通或绿，另一题不低于黄；否则执行降载规则。
- 第 26 天：检查第 22-25 天的四道主练题，至少两题能在 2 分钟内说出题型、不变量和复杂度。
- 第 33 天：主练题中至少 40% 已在延迟复测中变绿；若不足，第 34-35 天的伴练改为补红题。
- 第 44 天：陌生题能在 5 分钟内提出合理的朴素方案，且两道模拟题至少完整写出一道，才算达到基本面试线。

## 12. 为什么这样安排：科学依据与边界

这份计划依据通用学习科学研究设计，但这些研究并非专门针对 LeetCode 学习者，因此它只能提供更可靠的训练方法，不能保证面试结果。

- **提取练习**：主动回忆比反复阅读更有利于长期保持，因此每日先做复习卡、周六闭卷复写，而不是重看昨天代码。参考 [Roediger & Karpicke, 2006](https://pubmed.ncbi.nlm.nih.gov/16507066/)。
- **间隔效应**：主练题按 D+1、D+3、D+7、D+14 复习，避免同一天“看懂”造成的熟练错觉。参考 [Cepeda et al., 2006](https://pubmed.ncbi.nlm.nih.gov/16719566/)。
- **认知负荷与示例学习**：零基础阶段更早允许查看范例讲解，随后逐步把无提示思考从 10 分钟增加到 20 分钟；这比从第一天起长期硬想更适合新手。参考 [Sweller, 1988](https://link.springer.com/article/10.1007/BF00375122)。
- **交错与迁移**：前期按题型成组学习以建立模式，后期再混合题型，并使用两道只见过题面的陌生题检查迁移，避免只记住原题代码。参考 [Rohrer & Taylor, 2007](https://link.springer.com/article/10.1007/s11251-007-9015-8)。
- **恢复与可持续性**：周日缩短到 60 分钟，连续疲劳时降载。这里的目的不是最大化每天题量，而是提高 45 天内实际完成率。

最终结果以延迟复测和模拟表现为准，不以力扣提交数量为准。地图题只提供题型熟悉度，不能冒充会做；困难题不在本阶段目标内。
