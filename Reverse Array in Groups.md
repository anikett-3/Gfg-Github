## 01. Reverse Array in Groups

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/reverse-array-in-groups0255/1)

### Problem Description

**Task:** Given an integer array arr[] and an integer k, reverse every consecutive group of k elements. If fewer than k elements remain at the end, reverse all of them.Examples:Input: arr[] = [1, 2, 3, 4, 5], k = 3Output: [3, 2, 1, 5, 4]

#### Examples

##### Example 1

- **Explanation:** First group consists of elements 1, 2, 3. Second group consists of 4, 5.Input: arr[] = [5, 6, 8, 9], k = 5Output: [9, 8, 6, 5]Explnation: Since k is greater than the number of remaining elements, the entire array is reversed.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (Python)

- **Submitted:** 2026-11-13 21:11:46
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def reverseInGroups(self, arr, k):
        n = len(arr)

        for i in range(0, n, k):
            left = i
            right = min(i + k - 1, n - 1)

            while left < right:
                arr[left], arr[right] = arr[right], arr[left]
                left += 1
                right -= 1

        return arr
```

#### Solution 2 (Python)

- **Submitted:** 2026-11-13 21:10:37
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def reverseInGroups(self, arr, k):
        n = len(arr)

        for i in range(0, n, k):
            left = i
            right = min(i + k - 1, n - 1)

            while left < right:
                arr[left], arr[right] = arr[right], arr[left]
                left += 1
                right -= 1

        return arr
```

*Generated on: 11/13/2026, 9:12:45 PM*