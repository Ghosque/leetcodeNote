# 82.删除排序链表中的重复元素 II —— 链表

### 题目内容与要求

给定一个排序链表，删除所有含有重复数字的节点，只保留原始链表中 没有重复出现 的数字。

示例 1:
```
输入: 1->2->3->3->4->4->5
输出: 1->2->5
```

示例 2:
```
输入: 1->1->1->2->3
输出: 2->3
```

> 来源：力扣（LeetCode）\
链接：https://leetcode-cn.com/problems/remove-duplicates-from-sorted-list-ii

### 题解

本题要求是删除重复出现的数字，因此我们可以通过两个列表保存数据，一个是无重复的列表，一个是出现了重复数字的列表。

遍历链表，当数字出现在重复列表中时直接跳过操作；当数字出现在无重复列表时，表示已出现重复，将数字从无重复列表中删除，再添加到重复列表中；其余情况将当前节点的值添加到无重复列表中。

最终遍历无重复列表，生成新的链表并返回。
