## 01. Replace all 0's with 5

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/replace-all-0s-with-5/1)

### Problem Description

**Task:** You are given an integer n. You need to convert all zeroes of n to 5.

#### Examples

##### Example 1

- **Input:**
```text
n = 1004
```
- **Output:**
```text
1554
```
- **Explanation:** There are two zeroes in 1004 on replacing all zeroes with 5, the new number will be 1554.

##### Example 2

- **Input:**
```text
n = 121
```
- **Output:**
```text
121
```
- **Explanation:** Since there are no zeroes in 121, the number remains as 121.

#### Constraints

- **1.** `0 <= n <= 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(k)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-11 14:36:31
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def convertFive(self, n):
        # code here
        str_n=str(n)
        result=''
        for i in range(len(str_n)):
            if(str_n[i]=='0'):
                result=result+'5'
            else:
                result=result+str_n[i]
        return result
```

*Generated on: 10/22/2026, 12:50:23 AM*