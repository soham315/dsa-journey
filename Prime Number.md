## 01. Prime Number

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/prime-number2314/1)

### Problem Description

**Task:** Given a number n, determine whether it is a prime number or not.Note: A prime number is a number greater than 1 that has no positive divisors other than 1 and itself.Examples :Input: n = 7

#### Examples

##### Example 1

- **Output:**
```text
false
```
- **Explanation:** 1 has only one divisor (1 itself), which is not sufficient for it to be considered prime.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(sqrt(n))
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-18 14:25:08
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def isPrime(self, n):
        # code here
        
        if(n==0 or n==1):
            return False
        count=0
        for i in range(2,n//2):
            if(n % i == 0):
                return False
        else:
            return True
```

*Generated on: 10/22/2026, 12:54:22 AM*