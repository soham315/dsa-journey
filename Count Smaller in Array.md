## 01. Count Smaller in Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/count-of-smaller-elements5947/1)

### Problem Description

**Task:** Given an unsorted array arr[]. Find the count of elements less than or equal to the given element x.

#### Examples

##### Example 1

- **Input:**
```text
x = 9, arr[] = [10, 1, 2, 8, 4, 5]
```
- **Output:**
```text
5Explanation: The 5 elements are 1, 2, 8, 4 and 5.
```

##### Example 2

- **Input:**
```text
x = 2, arr[] = [1, 2, 2, 5, 7, 2, 9]
```
- **Output:**
```text
4 Explanation: The 4 elements are 1, 2, 2 and 2.
```

#### Constraints

- **1.** `1 <= arr.size() <= 10⁵`
- **2.** `1 <= a_i <= 10⁵`
- **3.** `0 <= x <= 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-21 14:36:27
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def countOfElements(self, x, arr):
        # code here
        count=0
        for i in range(len(arr)):
            if(arr[i]<=x):
                count+=1
            else:
                continue
        return count
```

*Generated on: 10/22/2026, 12:41:31 AM*