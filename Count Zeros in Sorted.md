## 01. Count Zeros in Sorted

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/count-the-zeros2550/1)

### Problem Description

**Task:** Given an array arr of only 0's and 1's. The array is sorted in such a manner that all the 1's are placed first and then they are followed by all the 0's. Find the count of all the 0's.

#### Examples

##### Example 1

- **Input:**
```text
arr[] = [1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0]
```
- **Output:**
```text
3
```
- **Explanation:** There are 3 0's in the given array.

##### Example 2

- **Input:**
```text
arr[] = [0, 0, 0, 0, 0]
```
- **Output:**
```text
5
```
- **Explanation:** There are 5 0's in the array.

#### Constraints

- **1.** `1 <= arr.size <= 10⁵`
- **2.** `0 <= arr[i] <= 1`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-21 22:04:59
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def countZeroes(self, arr):
        # code here
        count=0
        for i in arr:
            if i==0:
                count=count+1
            else:
                continue
        return count
```

*Generated on: 10/22/2026, 12:52:04 AM*