## 01. Largest in Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/largest-element-in-array4009/1)

### Problem Description

**Task:** Given an array arr[]. The task is to find the largest element and return it.Examples:Input: arr[] = [1, 8, 7, 56, 90]

#### Examples

##### Example 1

- **Output:**
```text
10
```
- **Explanation:** There is only one element which is the largest.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-15 03:28:58
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def largest(self, arr):
        # code here
        pos_inf = float("-inf")
        largest=pos_inf
        for i in range(len(arr)):
            # largest=arr[i]
            if(arr[i]>largest):
                largest=arr[i]
            else:
                continue
        return largest
```

*Generated on: 10/22/2026, 12:48:20 AM*