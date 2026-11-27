## 01. Alternative Sorting

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/alternative-sorting1311/1)

### Problem Description

**Task:** Given an array arr of distinct integers. Rearrange the array in such a way that the first element is the largest and the second element is the smallest, the third element is the second largest and the fourth element is the second smallest, and so on.Examples:Input: arr[] = [7, 1, 2, 3, 4, 5, 6]

#### Examples

##### Example 1

- **Output:**
```text
[7, 1, 6, 2, 5, 3, 4]
```
- **Explanation:** The first element is first maximum and second element is first minimum and so on.

##### Example 2

- **Input:**
```text
arr[] = [1, 6, 9, 4, 3, 7, 8, 2]
```
- **Output:**
```text
[9, 1, 8, 2, 7, 3, 6, 4]Explanation: The first element is first maximum and second element is first minimum and so on.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n log n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-11-27 18:32:02
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def alternateSort(self, arr):
        arr.sort()

        result = []
        left, right = 0, len(arr) - 1

        while left <= right:
            if left <= right:
                result.append(arr[right])
                right -= 1

            if left <= right:
                result.append(arr[left])
                left += 1

        return result
```

*Generated on: 11/27/2026, 6:32:14 PM*