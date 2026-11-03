## 01. Taking Input

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/taking-input/1)

### Problem Description

**Task:** You need to perform three separate tasks based on the given input:
String Input and Print: Read a string s (which may contain spaces) and print it as it is.
Integer Input and Print: Read an integer n and print it without any change.
Float Input and floor Print: Read a floating-point number as input, take its floor value, and print as an integer.

#### Examples

##### Example 1

- **Input:**
```text
s = "Hello", n = 20, f = 5.5Output: Hello 20 5Explanation: The string Hello is printed as it is. The integer 20 is printed without any change.For floating-point number 5.5, its floor value 5 is printed.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (Python)

- **Submitted:** 2026-09-09 22:05:03
- **Status:** Correct
- **Marks:** 0

```python
import math

# s to store string
# n to store integer
# f to store float
# ff  # To Store floor of float variable f


s = input()
n = int(input())
ff = float(input())
print(s)
print(n)
print(int(ff))
```

#### Solution 2 (Python)

- **Submitted:** 2026-09-08 21:55:01
- **Status:** Correct
- **Marks:** 1

```python
import math

# s to store string
# n to store integer
# f to store float
# ff  # To Store floor of float variable f

# code here
s = input()
n = int(input())
ff = float(input())
print(s)
print(n)
print(int(ff))
```

*Generated on: 11/3/2026, 6:01:12 PM*