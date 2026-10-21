## 01. Remove Common and Concat

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/remove-common-characters-and-concatenate-1587115621/1)

### Problem Description

**Task:** Given two strings, s1 and s2. The task is to remove all characters that are common in both strings and then combine the remaining characters from each string to form a new string.
The characters that are not shared between the two strings should appear in the result in the same order as they appear in their respective original strings.
If no characters are left after removing the common characters, return "-1"

#### Examples

##### Example 1

- **Input:**
```text
s1 = aacdb, s2 = gafd
```
- **Output:**
```text
cbgf
```
- **Explanation:** The common characters of s1 and s2 are: a, d. The uncommon characters of s1 and s2 are c, b, g and f. Thus the modified string with uncommon characters concatenated is cbgf.

##### Example 2

- **Input:**
```text
s1 = abcs, s2 = cxzca
```
- **Output:**
```text
bsxz
```
- **Explanation:** The common characters of s1 and s2 are: a,c. The uncommon characters of s1 and s2 are b,s,x and z. Thus the modified string with uncommon characters concatenated is bsxz.

#### Constraints

- **1.** `1 <= |Length of Strings| <= 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-21 04:12:55
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def concatenatedString(self,s1,s2):
        #code here

        set1 = set(s1)
        set2 = set(s2)
        result=[]
        for char in s1:
            if char not in s2:
                result.append(char)
        for char in s2:
            if char not in s1:
                result.append(char)
        final="".join(result)
        
        if (len(result)==0):
            return -1
        else:
            return final
```

*Generated on: 10/22/2026, 12:43:37 AM*