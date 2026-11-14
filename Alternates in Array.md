## 01. Alternates in Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-alternate-elements-of-an-array/1)

### Problem Description

**Task:** You are given an array arr[], the task is to return a list elements of arr in alternate order (starting from index 0).Examples:Input: arr[] = [1, 2, 3, 4]Output: 1 3Explanation:Take first element: 1Skip second element: 2Take third element: 3Skip fourth element: 4Input: arr[] = [1, 2, 3, 4, 5]

#### Examples

##### Example 1

- **Output:**
```text
1 3 5Explanation:Take first element: 1Skip second element: 2Take third element: 3Skip fourth element: 4Take fifth element: 5
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-11-14 10:04:54
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def getAlternates(self, arr):
        return arr[::2]
```

*Generated on: 11/14/2026, 10:06:30 AM*