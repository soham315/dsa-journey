## 01. Concatenate a List of Characters

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/convert-a-list-of-characters-into-a-string5142/1)

### Problem Description

**Task:** Given an array arr[] of lower case English characters as strings, merge all of them into a string. Note that the size of every string in the input array is 1 only.

#### Examples

##### Example 1

- **Input:**
```text
arr[] = ["g", "e", "e", "k", "s", "f", "o", "r", "g", "e", "e", "k", "s"]
```
- **Output:**
```text
geeksforgeeks
```
- **Explanation:** combined all the characters to form a single string.

##### Example 2

- **Input:**
```text
arr[] = ["e", "e", "b", "a"]
```
- **Output:**
```text
eeba
```
- **Explanation:** combined all the characters to form a single string.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-20 22:56:18
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def charToStr(self, arr):
        # code here
        res=[]
        for i in range(len(arr)):
            res.append(arr[i])
        new_res="".join(res)
        return new_res
```

*Generated on: 10/22/2026, 12:45:34 AM*