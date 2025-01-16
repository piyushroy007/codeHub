## Pattern 5:

Input: ‘N’ = 3

Output: 

  *
 ***
*****

## Solution :

void nStarTriangle(int n) {
    for(int i=1; i<=n; i++){
        for( int j=i; j<n; j++){
            cout<<" ";
        }
        for( int k=1;k<=i;k++){
            cout<<"*";
        }
        for(int l=1; l<=i-1;l++){
            cout<<"*";
        }
        for( int j=i; j<n; j++){
            cout<<" ";
        }
        cout<<endl;
    }
}

