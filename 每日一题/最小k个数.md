# title
面试题40. 最小的k个数
# description
输入整数数组 arr ，找出其中最小的 k 个数。例如，输入4、5、1、6、2、7、3、8这8个数字，则最小的4个数字是1、2、3、4。
# example
示例 1：

输入：arr = [3,2,1], k = 2
输出：[1,2] 或者 [2,1]


示例 2：
输入：arr = [0,1,2,1], k = 1
输出：[0]

来源：力扣（LeetCode）
链接：https://leetcode-cn.com/problems/zui-xiao-de-kge-shu-lcof

# solution
这是我在leetcode刷的第一道题目，遇到过的算法题最简单的一道题。思路就是1.直接排序2.截取k个数字。
# code
```
var getLeastNumbers = function(arr, k) {
    arr.sort((a,b)=>a-b)
    return arr.slice(0,k)
};
```

