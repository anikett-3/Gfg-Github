## 01. Sum of Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/sum-all-array-elements/1)

### Problem Description

**Task:** Given an integer array arr[], return the sum of all elements of arr.Examples:Input: arr[] = [1, 2, 3, 4]

#### Examples

##### Example 1

- **Output:**
```text
10
```
- **Explanation:** 1 + 2 + 3 + 4 = 10.

##### Example 2

- **Input:**
```text
arr[] = [1, 3, 3]
```
- **Output:**
```text
7
```
- **Explanation:** 1 + 3 + 3 = 7.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (6)

#### Solution 1 (Java)

- **Submitted:** 2026-11-15 20:37:19
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    public int arraySum(int arr[]) {
        // code here
        int sum = 0;
        for(int i = 0 ;i<arr.length;i++){ // for loop
            sum = sum+arr[i];
            
        }
        return sum; // return here
                                                                       
    }
}
```

#### Solution 2 (Java)

- **Submitted:** 2026-10-04 22:03:55
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    public int arraySum(int arr[]) {
        // code here
        int sum = 0;
        for(int i = 0 ;i<arr.length;i++){ // for loop
            sum = sum+arr[i];
            
        }
        return sum; // return here
                                                                       
    }
}
```

#### Solution 3 (Java)

- **Submitted:** 2026-09-14 23:21:29
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    public int arraySum(int arr[]) {
        // code here
        int sum = 0;
        for(int i = 0 ;i<arr.length;i++){
            sum = sum+arr[i];
            
        }
        return sum;
                                                                       
    }
}
```

#### Solution 4 (Java)

- **Submitted:** 2026-08-22 21:37:37
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    public int arraySum(int arr[]) {
        // code here
        int sum =0;
        for (int i = 0; i<=arr.length-1;i++){
            sum = sum+arr[i];
        }
        return sum;
    }
}
```

#### Solution 5 (Java)

- **Submitted:** 2026-08-21 22:57:09
- **Status:** Correct
- **Marks:** 0

```java
class Solution {
    public int arraySum(int arr[]) {
        // code here
        int sum =0;
        for (int i = 0; i<=arr.length-1;i++){
            sum = sum+arr[i];
        }
        return sum;
    }
}
```

#### Solution 6 (Java)

- **Submitted:** 2026-07-06 11:45:39
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int arraySum(int arr[]) {
        // code here
        int sum = 0;
        for(int i = 0 ;i<arr.length;i++){ // for loop
            sum = sum+arr[i];
            
        }
        return sum; // return here
                                                                       
    }
}
```

*Generated on: 11/15/2026, 8:37:54 PM*