## 01. Reverse a String

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/reverse-a-string/1)

### Problem Description

**Task:** Given a string s, reverse the string.Examples:Input: s = "Geeks"

#### Examples

##### Example 1

- **Output:**
```text
"skeeG"
```

##### Example 2

- **Input:**
```text
s = "for"
```
- **Output:**
```text
"a"
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (Python)

- **Submitted:** 2026-10-18 14:59:59
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def reverseString(self, s: str) -> str:
        # code here
        # reverse_str=s[::-1]
        # return reverse_str
        start=len(s)-1
        end=-1
        step=-1
        result='' #creating an empty string where we can add the reverse string elements
        for i in range(start,end,step):
            result=result+s[i]
        return result
```

#### Solution 2 (Python)

- **Submitted:** 2026-10-18 14:39:32
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def reverseString(self, s: str) -> str:
        # code here
        reverse_str=s[::-1]
        return reverse_str
```

*Generated on: 10/22/2026, 12:47:26 AM*