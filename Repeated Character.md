## 01. Repeated Character

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/repeated-character2058/1)

### Problem Description

**Task:** Given a string s consisting of lowercase English letters, find the first character that repeats in the string.Note: If the string contains no repeating characters, return '#'.Examples :Input: s = "geeksforgeeks"

#### Examples

##### Example 1

- **Output:**
```text
g
```
- **Explanation:** g, e, k and s are the repeating characters. Out of these, g occurs first.

##### Example 2

- **Input:**
```text
s = "abcde"
```
- **Output:**
```text
'#'
```
- **Explanation:** No repeating character present, so return '#'.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-20 14:54:01
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def firstRep(self, s: str) -> str:
        # code here
        repeated={}
        for char in s:
            if char in repeated:
                repeated[char]+=1
            else:
                repeated[char]=1
        
        for key,value in repeated.items():
            if value>1:
                return key
            else:
                continue
        return '#'
```

*Generated on: 10/22/2026, 12:53:29 AM*