# 54.螺旋矩阵

### 题目内容与要求

给定一个包含 m x n 个元素的矩阵（m 行, n 列），请按照顺时针螺旋顺序，返回矩阵中的所有元素。

示例 1:
```
输入:
[
 [ 1, 2, 3 ],
 [ 4, 5, 6 ],
 [ 7, 8, 9 ]
]
输出: [1,2,3,6,9,8,7,4,5]
```

示例 2:
```
输入:
[
  [1, 2, 3, 4],
  [5, 6, 7, 8],
  [9,10,11,12]
]
输出: [1,2,3,4,8,12,11,10,9,5,6,7]
```

> 来源：力扣（LeetCode）\
链接：https://leetcode-cn.com/problems/spiral-matrix

### 题解

顺时针打印矩阵，可以通过记录当前移动方向和已遍历过的元素进行顺时针运动。

按照 `右 -> 下 -> 左 -> 上 -> 右` 的顺序进行。
