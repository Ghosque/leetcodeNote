# 92.反转链表 II —— 链表

### 题目内容与要求

反转从位置 m 到 n 的链表。请使用一趟扫描完成反转。

说明:

1 ≤ m ≤ n ≤ 链表长度。

示例:
```
输入: 1->2->3->4->5->NULL, m = 2, n = 4
输出: 1->4->3->2->5->NULL
```

> 来源：力扣（LeetCode）\
链接：https://leetcode-cn.com/problems/reverse-linked-list-ii

### 题解

本题是指定一段区间进行链表反转，有点类似第 **25** 题的 K 个一组反转。

遍历链表，当移动到 _m_ 位置时开始获取长度为 _n-m+1_ 的区间链表值，记录 _m-1_ 和 _n-m+2_ 两个节点，对获取到的值逆向链接，得到新链表。
