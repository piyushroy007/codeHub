## Pattern 6:


Input: ‘N’ = 3
Output: 

*****
 ***
  *

## Solution :

void nStarTriangle(int n) {
    for(int i=1; i<=n; i++){
        for( int j=1; j<i; j++){
            cout<<" ";
        }
        for( int k=n;k>=i;k--){
            cout<<"*";
        }
        for(int l=n-1; l>=i;l--){
            cout<<"*";
        }
        for( int m=1; m<i; m++){
            cout<<" ";
        }
        cout<<endl;
    }
}

