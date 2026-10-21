## 01. Count Types of Characters

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/count-type-of-characters3635/1)

### Problem Description

**Task:** Given a string s, count the occurrence of the following in it.
Lowercase characters
Uppercase characters
Special characters
Numeric Values

> **Note:** There are no white spaces in the string.

#### Examples

##### Example 1

- **Input:**
```text
s = "#GeeKs01fOr@gEEks07"
```
- **Output:**
```text
[5, 8, 4, 2]
```
- **Explanation:** There are 5 uppercase characters, 8 lowercase characters, 4 numeric characters and 2 special characters.

##### Example 2

- **Input:**
```text
s = "*GeEkS4GeEkS*"
```
- **Output:**
```text
[6, 4, 1, 2]
```
- **Explanation:** There are 6 uppercase characters, 4 lowercase characters, 1 numeric character and 2 special characters.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (Python)

- **Submitted:** 2026-10-14 00:57:43
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def count (self,s):
        # your code here
        Lowercase_characters=0
        Uppercase_characters=0
        Numeric_Values=0
        Special_characters=0
        for i in range(len(s)):
            if(s[i].isupper()==True):
                Uppercase_characters+=1
            elif(s[i].islower()==True):
                Lowercase_characters+=1
            elif(s[i].isdigit()==True):
                Numeric_Values+=1
            else:
                Special_characters+=1
        return Uppercase_characters,Lowercase_characters,Numeric_Values,Special_characters
```

#### Solution 2 (Python)

- **Submitted:** 2026-10-14 00:57:36
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def count (self,s):
        # your code here
        Lowercase_characters=0
        Uppercase_characters=0
        Numeric_Values=0
        Special_characters=0
        for i in range(len(s)):
            if(s[i].isupper()==True):
                Uppercase_characters+=1
            elif(s[i].islower()==True):
                Lowercase_characters+=1
            elif(s[i].isdigit()==True):
                Numeric_Values+=1
            else:
                Special_characters+=1
        return Uppercase_characters,Lowercase_characters,Numeric_Values,Special_characters
```

*Generated on: 10/22/2026, 12:48:36 AM*