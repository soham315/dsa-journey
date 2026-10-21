## 01. One Odd Occuring

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/find-the-odd-occurence4820/1)

### Problem Description

**Task:** Given an array of arr[] positive integers where all numbers occur even number of times except one number which occurs odd number of times. Return that number.Examples:Input:arr[] = [1, 2, 3, 2, 3, 1, 3]

#### Examples

##### Example 1

- **Output:**
```text
3
```
- **Explanation:** 3 occurs three times.

##### Example 2

- **Input:**
```text
arr[] = [5, 7, 2, 7, 5, 2, 5]
```
- **Output:**
```text
5
```
- **Explanation:** 5 occurs three times.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (Python)

- **Submitted:** 2026-10-20 23:06:02
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def getOddOccurrence(self, arr):
        # code here 
        res={}
        for i in range(len(arr)):
            if arr[i] in res:
                res[arr[i]]+=1
            else:
                res[arr[i]]=1
        
        for key,val in res.items():
            if (val%2==1):
                return key
            else:
                continue
```

#### Solution 2 (Python)

- **Submitted:** 2026-10-20 23:03:47
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def getOddOccurrence(self, arr):
        # code here 
        res={}
        for i in arr:
            if i in res:
                res[i]+=1
            else:
                res[i]=1
        
        for key,val in res.items():
            if (val%2==1):
                return key
            else:
                continue
```

*Generated on: 10/22/2026, 12:45:19 AM*