## Pattern 16 :

Input: ‘N’ = 3

Output: 

    * * * * * * 
    * *     * * 
    *         * 
    *         * 
    * *     * * 
    * * * * * * 

## Solution :

    void symmetry(int N) {
        int iniS = 0;
        for(int i=0;i< N;i++){
            for(int j=1;j<=N-i;j++){
                cout<<"* ";
            }
            //for printing the spaces in the row.
            for(int j=0;j<iniS;j++){
                cout<<" ";
            }
            //for printing the stars in the row.
            for(int j=1;j<=N-i;j++){
                cout<<"* ";
            }
            iniS+=2;
            cout<<endl;
        }
        
        // for lower half of the pattern
        // initial spaces.
        iniS = 2*N -2;
        for(int i=1;i<=N;i++){
            //for printing the stars in the row.
            for(int j=1;j<=i;j++){
                cout<<"* ";
            }
            //for printing the spaces in the row.
            for(int j=0;j<iniS;j++){
                cout<<" ";
            }
            //for printing the stars in the row.
            for(int j=1;j<=i;j++){
                cout<<"* ";
            }
            iniS-=2;
            cout<<endl;
        }
    }