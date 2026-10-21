## 01. Check for Subsequence

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/given-two-strings-find-if-first-string-is-a-subsequence-of-second/1)

### Problem Description

**Task:** Given two strings s1 and s2. You have to check that s1 is a subsequence of s2 or not. Note: A subsequence is a sequence that can be derived from another sequence by deleting some elements without changing the order of the remaining elements.

#### Examples

##### Example 1

- **Input:**
```text
s1 = "AXY", s2 = "YADXCP"
```
- **Output:**
```text
false
```
- **Explanation:** s1 is not a subsequence of s2 as 'Y' appears before 'A'.

##### Example 2

- **Input:**
```text
s1 = "gksrek", s2 = "geeksforgeeks"
```
- **Output:**
```text
true
```
- **Explanation:** If we combine the bold character of "geeksforgeeks", it equals to s1. So s1 is a subsequence of s2.

#### Constraints

- **1.** `1 ≤ s1.size(), s2.size() ≤ 10⁶`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (Python)

- **Submitted:** 2026-10-21 03:51:28
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def isSubSeq(self, s1, s2):
        # code here
        start=0
        count=0
        for char in s1:
            if start<len(s2):
                for i in range(start,len(s2)):
                    if s2[i]==char:
                        start=i+1
                        count=count+1
                        break
                    else:
                        continue
        if(count==len(s1)):
            return True
        else:
            return False
```

#### Solution 2 (Python)

- **Submitted:** 2026-10-21 03:42:06
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def isSubSeq(self, s1, s2):
        # code here
        start=0
        count=0
        for char in s1:
            if start<len(s2):
                for i in range(start,len(s2)):
                    if char == s2[i]:
                        start = i+1
                        count=count+1
                        break
                    else:
                        continue
        if (count == len(s1)):
            return True
        else:
            return False
```

*Generated on: 10/22/2026, 12:52:34 AM*