## 01. For Loop

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/java-loops-set-11726/1)

### Problem Description

**Task:** Given a number n, print the first n positive even numbers in increasing order in a single line using a for loop.Examples:Input: n = 2

#### Examples

##### Example 1

- **Output:**
```text
2 4 6 8 10 12
```
- **Explanation:** The first 6 positive even numbers are 2, 4, 6, 8, 10 and 12.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-11-10 20:21:30
- **Status:** Correct
- **Marks:** 1

```python
if __name__ == "__main__":
    n = int(input())

    for i in range(1, n + 1):
        print(i * 2, end=" " if i < n else "")
```

*Generated on: 11/10/2026, 8:21:51 PM*