## 01. Rotate Array by One

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/cyclically-rotate-an-array-by-one2614/1)

### Problem Description

**Task:** Given an array arr[], rotate the array by one position in clockwise direction.Examples:Input: arr[] = [1, 2, 3, 4, 5]

#### Examples

##### Example 1

- **Output:**
```text
[3, 9, 8, 7, 6, 4, 2, 1]Explanation: After rotating clock-wise 3 comes in first position.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-11-11 19:16:15
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def rotate(self, arr: list[int]) -> None:
        if len(arr) <= 1:
            return

        last = arr[-1]

        for i in range(len(arr) - 1, 0, -1):
            arr[i] = arr[i - 1]

        arr[0] = last
```

*Generated on: 11/11/2026, 7:16:54 PM*