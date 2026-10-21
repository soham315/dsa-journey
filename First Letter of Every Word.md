## 01. First Letter of Every Word

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-first-letter-of-every-word-in-the-string3632/1)

### Problem Description

**Task:** Given a string s, the task is to create a string with the first letter of every word in the string. The string s contains lower case English alphabets and its words have a single space between them.

#### Examples

##### Example 1

- **Input:**
```text
s = "geeks for geeks"
```
- **Output:**
```text
gfgExplanation: First word starts at index 0, take 'g' After first space, next word starts with 'f'After second space, next word starts with 'g'
```

##### Example 2

- **Input:**
```text
s = "bad is good"
```
- **Output:**
```text
big
```

#### Constraints

- **1.** `1 ≤ |s| ≤ 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(|S|)
- **Expected Auxiliary Space Complexity:** O(|S|)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-21 14:21:50
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def firstAlphabet(self, s):
        # code here
        new_list=s.split(" ")
        res=[]
        for i in range(len(new_list)):
            res.append(new_list[i][0])
        output="".join(res)
        return output
```

*Generated on: 10/22/2026, 12:42:58 AM*