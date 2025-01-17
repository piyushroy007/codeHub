## Pattern 14 :

Input: ‘N’ = 3

Output: 

        A
      A B A
    A B C B A

## Solution in C++:

    void alphaHill(int n) {
        for (int i = 1; i <= n; i++){
            for(int k = n*2; k > i*2; k--){
                cout << " ";
            }
            for(char j = 'A'; j <= 'A'+(i-1); j++){
                cout << j << " ";
            }
            for(char j = 'A'+(i-2); j >= 'A'; j--){
                cout << j << " ";
            }
            for (int k = n; k >= i; k--) {
                cout << " ";
            }
            cout << endl;
        }
    }