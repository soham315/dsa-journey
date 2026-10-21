## 01. First and Last in Sorted

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/first-and-last-occurrences-of-x3116/1)

### Problem Description

**Task:** Given a sorted array arr[] with possibly some duplicates, find the first and last occurrences of an element x in the given array.Note: If the number x is not found in the array then return both the indices as -1.Examples:Input: arr[] = [1, 3, 5, 5, 5, 5, 67, 123, 125], x = 5

#### Examples

##### Example 1

- **Output:**
```text
[2, 5]
```
- **Explanation:** First occurrence of 5 is at index 2 and last occurrence of 5 is at index 5

##### Example 2

- **Input:**
```text
arr[] = [1, 3, 5, 5, 5, 5, 7, 123, 125], x = 7
```
- **Output:**
```text
[-1, -1]
```
- **Explanation:** No occurrence of 4 in the array, so, output is [-1, -1]

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-21 22:23:50
- **Status:** Correct
- **Marks:** 4

```python
class Solution:
    def find(self, arr, x):
        # code here
        result_index=[]
        n=len(result_index)
        
        for i in range(len(arr)):
            if(arr[i]==x):
               result_index.append(i)
            else:
                continue
        
        if(len(result_index)==0):
            return -1,-1
        first_occurance = result_index[0]
        last_occurance = result_index[-1]

        return first_occurance, last_occurance
```

*Generated on: 10/22/2026, 12:40:56 AM*