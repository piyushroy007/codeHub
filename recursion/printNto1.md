## Print N to 1 without loop


Print numbers from N to 1 (space separated) without the help of loops.

Example 1:

    Input:
    N = 10
    Output: 10 9 8 7 6 5 4 3 2 1

## Solution in C++ :

    void printNos(int N) {
        if(N <=0) return;
        cout<<N<< " ";
        printNos(N-1);
    }