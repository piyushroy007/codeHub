## Pattern 2:


Input: ‘N’ = 3

Output: 
1
2 2 
3 3 3

## Solution :

void triangle(int n) {
    for(int i=1;i<=n;i++){
        for( int j=1;j<=i; j++){
            cout << i << " ";
        }
        cout<< endl;
    }
}

