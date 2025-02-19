## 509. Fibonacci Number

The Fibonacci numbers, commonly denoted F(n) form a sequence, called the Fibonacci sequence, such that each number is the sum of the two preceding ones, starting from 0 and 1. That is,

F(0) = 0, F(1) = 1
F(n) = F(n - 1) + F(n - 2), for n > 1.
Given n, calculate F(n).

Example 1:

    Input: n = 2
    Output: 1
    Explanation: F(2) = F(1) + F(0) = 1 + 0 = 1.

Example 2:

    Input: n = 3
    Output: 2
    Explanation: F(3) = F(2) + F(1) = 1 + 1 = 2.

## Solution in c++ :

    int fib(int n) {
        if (n < 2) {
            return n;
        }
        int p = 0, q = 0, r = 1;
        for (int i = 2; i <= n; ++i) {
            p = q;
            q = r;
            r = p + q;
        }
        return r;
    }

## 2nd solution :

    int main()
    {
            int n=0;
            cin>>n;
            int first=0;
            int second=1;
            int third=0;
            if(n<2){
                    cout<<n;
                    return 0;
            }
            for(int i=2;i<=n;i++){
                    third=first+second;
                    first=second;
                    second=third;
            }
            cout<< third;
            return 0;
    }
