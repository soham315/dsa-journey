## 01. Palindrome Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/perfect-arrays4645/1)

### Problem Description

**Task:** Given an array arr[], the task is to find whether the arr is palindrome or not. An array is said to be palindrome if its reverse array matches the original array.

#### Examples

##### Example 1

- **Input:**
```text
arr = [1, 2, 3, 2, 1]
```
- **Output:**
```text
true
```
- **Explanation:** If we reverse, we get [1, 2, 3, 2, 1] which is the same as before. So, the answer is true.

##### Example 2

- **Input:**
```text
arr = [1, 2, 3, 4, 5]
```
- **Output:**
```text
falseExplanation: If we reverse it, we get [5, 4, 3, 2, 1] which is the not same as before. So, the answer false.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-20 12:41:01
- **Status:** Correct
- **Marks:** 1

```python
import copy
class Solution:
    def isPalindrome(self, arr):
        # code here
        rev_arr = copy.deepcopy(arr)

        i=0
        j=len(rev_arr)-1
        
        while(i<j):
            rev_arr[i],rev_arr[j]=rev_arr[j],rev_arr[i]
            i=i+1
            j=j-1
        if(rev_arr == arr):
            return True
        else:
            return False
```

*Generated on: 10/22/2026, 12:47:09 AM*