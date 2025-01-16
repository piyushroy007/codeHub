## Pattern 8:

Input: ‘N’ = 3

Output: 

1
0 1
1 0 1

## Solution:

void nBinaryTriangle(int n) {
    int row=1;
    for(int i=1; i<=n; i++){
        int col =row;
        for(int j=1; j<=i; j++){
            cout<< col <<" ";
            if( col == 1){
                col =0;
            } else {
                col = 1;
            }
        }
        cout << "\n";
        if( row == 1){
            row =0;
        } else {
            row = 1;
        }
    }
}

