## 01. Second Largest

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/second-largest3735/1)

### Problem Description

**Task:** Given an array of positive integers arr[], return the second largest element from the array. If the second largest element doesn't exist then return -1.Note: The second largest element should not be equal to the largest element.Examples:Input: arr[] = [12, 35, 1, 10, 34, 1]

#### Examples

##### Example 1

- **Output:**
```text
-1
```
- **Explanation:** The largest element of the array is 10 and the second largest element does not exist.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-21 16:46:20
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def getSecondLargest(self, arr):
        # code here
        largest = float('-inf')
        second_largest = float('-inf')
        
        n=len(arr)
        
        for i in range(0,n):
            if arr[i]>largest:
                second_largest=largest
                largest=arr[i]
            elif(arr[i]>second_largest and arr[i]!=largest):
                second_largest=arr[i]
                
        if(second_largest!=float('-inf')):
            return second_largest
        else:
            return -1
```

*Generated on: 10/22/2026, 12:41:15 AM*