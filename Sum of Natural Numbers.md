## 01. Sum of Natural Numbers

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/reverse-coding2452/1)

### Problem Description

**Task:** Given an integer n, compute the sum of all natural numbers from 1 to n (inclusive). If n is 0, the sum should be 0.Examples:Input: n = 6

#### Examples

##### Example 1

- **Output:**
```text
0
```
- **Explanation:** Since n is 0, the sum is 0.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-14 00:06:16
- **Status:** Correct
- **Marks:** 1

```python
n = int(input())

# code here
sum=0
if n==0:
    sum=0
for i in range(1,n+1):
    sum=sum+i
print(sum)
```

*Generated on: 10/22/2026, 12:49:31 AM*