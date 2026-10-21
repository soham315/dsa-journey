## 01. Non Repeating Character

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/non-repeating-character-1587115620/1)

### Problem Description

**Task:** Given a string s consisting of lowercase English Letters. return the first non-repeating character in s. If there is no non-repeating character, return '$'.Examples:Input: s = "geeksforgeeks"

#### Examples

##### Example 1

- **Output:**
```text
'f'
```
- **Explanation:** In the given string, 'f' is the first character in the string which does not repeat.Input: s = "racecar"Output: 'e'Explanation: In the given string, 'e' is the only character in the string which does not repeat.Input: s = "aabbccc"Output: '$'Explanation: All the characters in the given string are repeating.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-20 21:40:45
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def nonRepeatingChar(self,s):
        res={}
        for i in s:
            if i in res:
                res[i]+=1
            else:
                res[i]=1
        for key,value in res.items():
            if value==1:
                return key
            else:
                continue
        return '$'
```

*Generated on: 10/22/2026, 12:53:16 AM*