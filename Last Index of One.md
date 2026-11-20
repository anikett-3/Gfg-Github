## 01. Last Index of One

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/last-index-of-15847/1)

### Problem Description

**Task:** Given a string s consisting only of '0' and '1', find the last index at which '1' occurs. If '1' is not present in the string, return -1.Examples:Input: s = "01001"

#### Examples

##### Example 1

- **Output:**
```text
4
```
- **Explanation:** Last index of 1 in given string is 4.

##### Example 2

- **Input:**
```text
s = "0"
```
- **Output:**
```text
-1
```
- **Explanation:** Since, 1 is not present, so output is -1.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-11-20 07:21:40
- **Status:** Correct
- **Marks:** 1

```python
# class Solution:
#     def lastIndex(self, s: str) -> int:
#         # code here
        
        
class Solution:
    def lastIndex(self, s: str) -> int:
        return s.rfind('1')
```

*Generated on: 11/20/2026, 7:21:54 AM*