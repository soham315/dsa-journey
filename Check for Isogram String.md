## 01. Check for Isogram String

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/check-if-a-string-is-isogram-or-not-1587115620/1)

### Problem Description

**Task:** Given a string s of lowercase alphabets, check if it is Isogram or not. An Isogram is a string in which no letter occurs more than once.

#### Examples

##### Example 1

- **Input:**
```text
s = "machine"
```
- **Output:**
```text
true
```
- **Explanation:** "machine" is an Isogram as no letter has appeared twice. so we return true.

##### Example 2

- **Input:**
```text
s = "geeks"
```
- **Output:**
```text
false
```
- **Explanation:** "geeks" is not an Isogram as 'e' appears twice. so we return false.

#### Constraints

- **1.** `1 ≤ |s| ≤ 10³`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (3)

#### Solution 1 (Python)

- **Submitted:** 2026-10-20 14:40:26
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def isIsogram(self,s):
        
        # using set approach 
        #Your code here
        # s=list(s)
        # seen_set = set()
        
        # for i in range(len(s)):
        #     if s[i] in seen_set:
        #         return False
        #     else:
        #         seen_set.add(s[i])
        # return True
        
        res={} #create an empty dict to store the characters
        for i in s:
            if i in res:
                return False
            else:
                res[i]=1
        return True
```

#### Solution 2 (Python)

- **Submitted:** 2026-10-17 18:37:41
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def isIsogram(self,s):
        #Your code here
        # s=list(s)
        seen_set = set()
        
        for i in range(len(s)):
            if s[i] in seen_set:
                return False
            else:
                seen_set.add(s[i])
        return True
```

#### Solution 3 (Python)

- **Submitted:** 2026-10-17 18:34:43
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def isIsogram(self,s):
        #Your code here
        s=list(s)
        seen_set = set()
        
        for i in range(len(s)):
            if s[i] in seen_set:
                return False
            else:
                seen_set.add(s[i])
        return True
```

*Generated on: 10/22/2026, 12:53:56 AM*