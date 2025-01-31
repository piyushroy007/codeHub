## LCM And GCD

Given two integers a and b, write a function lcmAndGcd() to compute their LCM and GCD. The function inputs two integers a and b and returns a list containing their LCM and GCD.

## Examples:

    Input: a = 5 , b = 10
    Output: [10, 5]
    Explanation: LCM of 5 and 10 is 10, while their GCD is 5.

    Input: a = 14 , b = 8
    Output: [56, 2]
    Explanation: LCM of 14 and 8 is 56, while their GCD is 2.

## Solution in c++ :

        vector<int> lcmAndGcd(int a, int b) {
            int n1=a;
            int n2=b;
            int LCM=0;
            int gcd=0;
            while (a > 0 && b > 0) {
                if (a > b) {
                    a = a % b;
                }
                else {
                    b = b % a;
                }
            }
            
            gcd =(a==0)?b:a;
            LCM = (n1*n2)/gcd;
            return {LCM,gcd};
        }