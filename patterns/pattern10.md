## Pattern 10

Sample Input 3 :

7

Sample Output 3 :

    1
    2 3
    4 5 6 
    7 8 9 10
    11 12 13 14 15 
    16 17 18 19 20 21 
    22 23 24 25 26 27 28

## Solution in C++ :

    void nNumberTriangle(int n) {
        int c=1;
        for(int i=1; i<=n; i++){
            //number
            for(int j=1; j<=i; j++){
                cout << c << " ";
                c++;
            }
            //space
            for(int j=n-i; j>=1; j--){
                cout<< " ";
            }
            cout<< endl;
        }
    }