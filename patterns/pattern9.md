## Pattern 9:

Input: ‘N’ = 3

Output: 

1         1
1 2     2 1
1 2 3 3 2 1


## Solution in c++:

    void numberCrown(int n) {
        for(int i=1; i<=n; i++){
            //number
            for(int j=1; j<=i; j++){
                cout<< j <<" ";
            }
            //space
            for(int k=1; k<=2*(n-i); k++){
                cout<< " ";
            }
            //number
            for(int j=i; j>=1; j--){
                cout<< j <<" ";
            }
            cout<< endl;
        }
    }