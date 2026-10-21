## 01. Value Equal to Position

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/value-equal-to-index-value1330/1)

### Problem Description

**Task:** Given an array arr[], find the elements whose value is equal to the position where they appear.

> **Note:** There can be more than one element in the array which have the same value as its position. You need to include the position of every such element.

#### Examples

##### Example 1

- **Input:**
```text
arr[] = [15, 2, 45, 4, 7]
```
- **Output:**
```text
[2, 4]
```
- **Explanation:** Here, arr[2] = 2 exists here and arr[4] = 4 exists.

##### Example 2

- **Input:**
```text
arr[] = [1]
```
- **Output:**
```text
[1]
```
- **Explanation:** Here arr[1] = 1 exists.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-21 14:34:31
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def valEqualToPos(self, arr):
        # code here
        res=[]
        for i in range(len(arr)):
            if(i+1==arr[i]):
                res.append(arr[i])
            else:
                continue
        return res
```

*Generated on: 10/22/2026, 12:42:44 AM*