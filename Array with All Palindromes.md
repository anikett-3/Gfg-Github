## 01. Array with All Palindromes

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/palindromic-array-1587115620/1)

### Problem Description

**Task:** Given an array arr[] of positive integers. Return true if all the array elements are palindrome otherwise, return false.Examples:Input: arr[] = [111, 222, 333, 444, 555]

#### Examples

##### Example 1

- **Output:**
```text
false
```
- **Explanation:** 20 is not a palindrome hence the output is false.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-11-04 11:20:11
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def isPalinArray(self, arr):
        for num in arr:
            if str(num) != str(num)[::-1]:
                return False
        return True
```

*Generated on: 11/4/2026, 11:20:31 AM*