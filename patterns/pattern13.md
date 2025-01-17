## Pattern 13:

Sample Input 3 :

4

Sample Output 3 :

    A
    B B
    C C C
    D D D D

## Solution in C++ :

    void alphaRamp(int n) {
        char ch='A';
        for(int i=0;i<n;i++){
            for(int j=0;j<=i;j++){
                cout<< ch <<" ";
            }
            cout << endl;
            ch += 1;
        }
    }
