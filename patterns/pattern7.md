## Pattern 7:


Input: ‘N’ = 3

Output: 

*
**
***
**
*

## Solution : 

void nStarTriangle(int n) {
    //upper part
    for( int i=0; i<n; i++){
        for(int j=0; j<=i; j++){
            cout<<"*";
        }
        for(int k=0; k<n-i-1; k++){
            cout<<" ";
        }
        cout<< "\n";
    }
    //lower part
    for( int i=0; i<n-1; i++){
        for(int j=0; j<n-i-1; j++){
            cout<<"*";
        }
        for(int k=0; k<i; k++){
            cout<<" ";
        }
        cout<< "\n";
    }
}

