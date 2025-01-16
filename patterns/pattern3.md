## Pattern 3:

Input: ‘N’ = 3

Output: 
* * *
* *
*

## Solution : 

void seeding(int n) {
    for(int i=n; i>=1; i--){
        for(int j=i;j>=1;j--){
            cout << "* ";
        }
        cout << endl;
    }
}


