## Sum of first n terms

Given an integer n, calculate the sum of series 13 + 23 + 33 + 43 + … till n-th term.

Examples:

    Input: n = 5
    Output: 225
    Explanation: 13 + 23 + 33 + 43 + 53 = 225

    Input: n = 7
    Output: 784
    Explanation: 13 + 23 + 33 + 43 + 53 + 63 + 73 = 784

## Solution in c++ :

    int sumOfSeries(int n) {
        if(n == 0){
            return 0;
        }
        return pow(n,3) + sumOfSeries(n-1);
    }