## 01. Count Uppercase characters

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/find-the-camel3348/1)

### Problem Description

**Task:** Given a string s, count the total number of uppercase English letters present in it.Examples:Input: s = "ckjkUUYII"

#### Examples

##### Example 1

- **Output:**
```text
5
```
- **Explanation:** The uppercase characters present in the string are 'U', 'U', 'Y', 'I', and 'I'.

##### Example 2

- **Input:**
```text
s = "abcd"
```
- **Output:**
```text
0
```
- **Explanation:** There are no uppercase characters present in the string.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-14 00:35:10
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def countCamelCase(self, s: str) -> int:
        # code here
        new_str=list(s)
        count=0
        for i in range(len(new_str)):
            if(new_str[i].isupper()==True):
                count=count+1
            else:
                continue
        return count
```

*Generated on: 10/22/2026, 12:49:01 AM*