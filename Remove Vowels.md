## 01. Remove Vowels

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/remove-vowels-from-string1446/1)

### Problem Description

**Task:** Given a string s. Your task is to remove the vowels from the string.

#### Examples

##### Example 1

- **Input:**
```text
s = "welcome to geeksforgeeks"
```
- **Output:**
```text
"wlcm t gksfrgks"
```
- **Explanation:** Vowels were ignored only consonents were returned in the same order.

##### Example 2

- **Input:**
```text
s = "what is your name ?"
```
- **Output:**
```text
wht s yr nm ?
```

#### Constraints

- **1.** `1 <= |s| <= 10⁵Alphabets are lower cases only`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-21 14:54:23
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def removeVowels(self, s):
        # code here
        vowels="aeiouAEIOU"
        output=""
        for char in s:
            if char in vowels:
                continue
            else:
                output += char
        return output
```

*Generated on: 10/22/2026, 12:40:15 AM*