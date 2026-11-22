## 01. First 1 in Sorted Binary

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/index-of-first-1-in-a-sorted-array-of-0s-and-1s4048/1)

### Problem Description

**Task:** Given a sorted array arr consisting of 0s and 1s. The task is to find the index (0-based indexing) of the first 1 in the given array. NOTE: If one is not present then, return -1.Examples :Input : arr[] = [0, 0, 0, 0, 0, 0, 1, 1, 1, 1]

#### Examples

##### Example 1

- **Output:**
```text
6
```
- **Explanation:** The index of first 1 in the array is 6.

##### Example 2

- **Input:**
```text
arr[] = [0, 0, 0, 0]
```
- **Output:**
```text
-1
```
- **Explanation:** 1's are not present in the array.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-11-22 20:23:50
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def firstIndex(self, arr):
        low = 0
        high = len(arr) - 1
        ans = -1

        while low <= high:
            mid = (low + high) // 2

            if arr[mid] == 1:
                ans = mid
                high = mid - 1
            else:
                low = mid + 1

        return ans
```

*Generated on: 11/22/2026, 8:25:01 PM*