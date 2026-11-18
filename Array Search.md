## 01. Array Search

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/search-an-element-in-an-array-1587115621/1)

### Problem Description

**Task:** Given an array, arr[] of n integers, and an integer element x, find whether element x is present in the array. Return the index of the first occurrence of x in the array, or -1 if it doesn't exist.Examples:Input: arr[] = [1, 2, 3, 4], x = 3Output: 2

#### Examples

##### Example 1

- **Explanation:** For array [10, 8, 30, 4, 5], the element to be searched is 5 and it is at index 4. So, the output is 4.

##### Example 2

- **Input:**
```text
arr[] = [10, 8, 30], x = 6Output: -1
```
- **Explanation:** The element to be searched is 6 and it is not present, so we return -1.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-11-18 18:50:13
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def search(self, arr, x):
        for i in range(len(arr)):
            if arr[i] == x:
                return i
        return -1
```

*Generated on: 11/18/2026, 6:51:31 PM*