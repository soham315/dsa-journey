## 01. Count Odd and Even

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/count-odd-even/1)

### Problem Description

**Task:** Given an array arr[] of positive integers. The task is to return the count of the number of odd and even elements in the array.

> **Note:** Return two elements where the first one in the count of odd & second one is the count of even.

#### Examples

##### Example 1

- **Input:**
```text
arr[] = [1, 2, 3, 4, 5]
```
- **Output:**
```text
3 2
```
- **Explanation:** There are 3 odd elements (1, 3, 5) and 2 even elements (2 and 4).

##### Example 2

- **Input:**
```text
arr[] = [1, 1]
```
- **Output:**
```text
2 0Explanation: There are 2 odd elements (1, 1) and no even elements.
```

#### Constraints

- **1.** `1 <= arr.size <= 10⁶`
- **2.** `1 <= arr[i] <= 10⁶`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (Python)

- **Submitted:** 2026-10-11 14:12:41
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def countOddEven(self, arr):
        #Code here
        count_odd =0
        count_even=0
        
        
        for i in range(len(arr)):
            if(arr[i]%2==0):
                count_even = count_even+1
            else:
                count_odd = count_odd+1
    
        return count_odd,count_even
```

#### Solution 2 (Python)

- **Submitted:** 2026-10-11 14:05:46
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def countOddEven(self, arr):
        #Code here
        count_odd =0
        count_even=0
        output=" "
        
        for i in range(len(arr)):
            if(arr[i]%2==0):
                count_even = count_even+1
            else:
                count_odd = count_odd+1
    
        return count_odd,count_even
```

*Generated on: 10/22/2026, 12:50:45 AM*