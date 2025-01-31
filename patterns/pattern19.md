## Pattern 19

Input 

N = 3

Result: 

    3 3 3 3 3 
    3 2 2 2 3 
    3 2 1 2 3 
    3 2 2 2 3 
    3 3 3 3 3

## Solution in c++ : 

    void getNumberPattern(int n) {
        for(int i=0;i<2*n-1;i++){
            for(int j=0;j<2*n-1;j++){
                // Initialising the top, down, left and right indices of a cell.
                int top = i;
                int bottom = j;
                int right = (2*n - 2) - j;
                int left = (2*n - 2) - i;
                cout<<(n- min(min(top,bottom), min(left,right)));
            }
            cout<<endl;
        }
    }