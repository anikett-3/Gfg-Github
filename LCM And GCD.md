## 01. LCM And GCD

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/lcm-and-gcd4516/1)

### Problem Description

**Task:** Given two integers a and b, You have to compute their LCM and GCD and return an array containing their LCM and GCD.Examples:Input: a = 5 , b = 10

#### Examples

##### Example 1

- **Output:**
```text
[1, 1]
```
- **Explanation:** LCM of 1 and 1 is 1, while their GCD is 1.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log(min(a, b))
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-11-05 20:16:50
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def lcmAndGcd(self, a: int, b: int) -> List[int]:

        x, y = a, b

        # Calculate GCD using Euclidean Algorithm
        while y != 0:
            x, y = y, x % y

        gcd = x

        # Calculate LCM
        lcm = (a * b) // gcd

        return [lcm, gcd]
```

*Generated on: 11/5/2026, 8:17:21 PM*