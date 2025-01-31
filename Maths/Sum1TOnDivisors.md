## Sum 1 to n Divisors

Given a positive integer n, The task is to find the value of Σi F(i) where i is from 1 to n and function F(i) is defined as the sum of all divisors of i.

Examples:

    Input: n = 4
    Output: 15
    Explanation:
    F(1) = 1
    F(2) = 1 + 2 = 3
    F(3) = 1 + 3 = 4
    F(4) = 1 + 2 + 4 = 7
    So, F(1) + F(2) + F(3) + F(4)
        = 1 + 3 + 4 + 7 = 15

    Input: n = 5
    Output: 21
    Explanation:
    F(1) = 1
    F(2) = 1 + 2 = 3
    F(3) = 1 + 3 = 4
    F(4) = 1 + 2 + 4 = 7
    F(5) = 1 + 5 = 6
    So,  F(1) + F(2) + F(3) + F(4) + F(5)
        = 1 + 3 + 4 + 7 + 6 = 21

## Solution in c++ :

    int sumOfDivisors(int n) {
        int sum = 0;
        
        for(int i=1; i <= n; i++){
            
            sum += (n/i) * i;
        }
        return sum;
    }

## Note :

here is our pattern that for any N 
ans = (1 x (N/1)) + (2 x (N/2)) + (3x(N/3)) + ... + (Nx(N/N)) 

https://www.geeksforgeeks.org/problems/sum-of-all-divisors-from-1-to-n4738/1
