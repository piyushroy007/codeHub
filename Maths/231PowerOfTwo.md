## 231. Power of Two

Given an integer n, return true if it is a power of two. Otherwise, return false.

An integer n is a power of two, if there exists an integer x such that n == 2x.


## Example 1:

Input: n = 1
Output: true
Explanation: 20 = 1

## Example 2:

Input: n = 16
Output: true
Explanation: 24 = 16

## Example 3:

Input: n = 3
Output: false

## Solution in C++ :

    class Solution {
    public:
        bool isPowerOfTwo(int n) {
            if (n == 0) {
                return false;
            }
            while ((n & 1) == 0) {
                n >>= 1;
            }
            return (n == 1);
        }
    };

## Note :

we introduce a while loop to use constant space, we use bit operation n >>= 1; to divide n by 2, but it is equivalent to n /= 2; (I don’t think the compiler makes a difference). Similarly there are 2 ways to check if n is divisible by 2: (n & 1) == 0 or n % 2 == 0.