## 01. Change the Case based on First Character

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/change-the-string3541/1)

### Problem Description

**Task:** Given a string s, the task is to change the complete string to uppercase or lowercase depending on the case of the first character.

#### Examples

##### Example 1

- **Input:**
```text
s = "abCD"
```
- **Output:**
```text
"abcd"
```
- **Explanation:** The first letter (a) is lowercase. Hence, the complete string is made lowercase.

##### Example 2

- **Input:**
```text
s = "Abcd"
```
- **Output:**
```text
"ABCD"
```
- **Explanation:** The first letter (A) is uppercase. Hence, the complete string is made uppercase.

#### Constraints

- **1.** `1 <= |s| <= 10⁴`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-13 00:02:29
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def modify(self, s):
        # code here
        if s[0].isupper()==True:
            s=s.upper()
        else:
            s=s.lower()
    
        return s
```

*Generated on: 10/22/2026, 12:49:54 AM*