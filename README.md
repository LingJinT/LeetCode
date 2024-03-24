# LeetCode
LeetCode刷题记录

## 数组
### (1)二分查找
[LeetCode](https://leetcode.cn/problems/binary-search/)
```ts
function search(nums: number[], target: number): number {
  let left = 0
  let right = nums.length - 1
  while(left <= right) {
    let mid = Math.ceil((left + right) / 2)
    if(nums[mid] === target) {
      return mid
    }
    if(nums[mid] < target) {
      left = mid + 1
    } else {
      right = mid - 1
    }
  }
  return -1
};
```
