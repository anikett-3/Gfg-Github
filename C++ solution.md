## 01. C++ solution

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/maximum-perimeter-of-triangle-from-array4322/1)

### Problem Description

**Task:** Given an array arr[] of positive integers. Find out the maximum perimeter of the triangle from the array.Examples:Input: arr[] = [6, 1, 6, 5, 8, 4]

#### Examples

##### Example 1

- **Output:**
```text
20
```
- **Explanation:** Triangle formed by 8,6 & 6. Thus perimeter 20.

##### Example 2

- **Input:**
```text
arr[] = [7, 55, 20, 1, 4, 33, 12]
```
- **Output:**
```text
-1
```
- **Explanation:** As the triangle is not possible because the condition: the sum of two sides should be greater than third is not fulfilled here.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-11-28 19:48:50
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def maxPerimeter(self, arr):
        arr.sort(reverse=True)

        for i in range(len(arr) - 2):
            a, b, c = arr[i], arr[i + 1], arr[i + 2]

            if b + c > a:
                return a + b + c

        return -1
```

*Generated on: 11/28/2026, 7:50:43 PM*