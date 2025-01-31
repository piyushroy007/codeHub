## Pattern 18

Sample Input 2 :

5

Sample Output 2 :

    *****
    *   *
    *   *
    *   *
    *****

## Solution in C++ :

    void getStarPattern(int n) {
        // outer loop for no. of rows.
        for(int i=0;i<n;i++){
            // inner loop for printing the stars at borders only.
            for(int j=0;j<n;j++){
                if(i==0 || j==0 || i==n-1 || j==n-1)
                cout<<"*";
                // if not border index, print space.
                else cout<<" ";
            }
            cout<<endl;
        }
    }
