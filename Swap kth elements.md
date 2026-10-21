## 01. Swap kth elements

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/swap-kth-elements5500/1)

### Problem Description

**Task:** Given an array arr[], swap the k^th element from the beginning with the k^th element from the end.

> **Note:** 1-based indexing is followed.

#### Examples

##### Example 1

- **Input:**
```text
arr[] = [1, 2, 3, 4, 5, 6, 7, 8], k = 3
```
- **Output:**
```text
[1, 2, 6, 4, 5, 3, 7, 8]
```
- **Explanation:** 3^rd element from beginning is 3 and 3rd element from end is 6, so we replace 3 & 6.

##### Example 2

- **Input:**
```text
arr[] = [5, 3, 6, 1, 2], k = 2
```
- **Output:**
```text
[5, 1, 6, 3, 2]
```
- **Explanation:** 2^nd element from beginning is 3 and from end is 1.

#### Constraints

- **1.** `1 ≤ arr.size(), k ≤ 10⁶-10⁹ ≤ arr[i] ≤ 10⁹`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-18 14:35:12
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def swapKth(self, arr, k):
        # Code Here
        arr[k-1],arr[-k]=arr[-k],arr[k-1]
        return arr
```

*Generated on: 10/22/2026, 12:47:44 AM*