## Pattern 12:

Sample Input 2 :

4

Sample Output 2 :

    A B C D
    A B C
    A B
    A

## Solution in C++:

    void nLetterTriangle(int n) {
        for(int i=0; i<n; i++){
            for(char ch='A'; ch<='A'+n-i-1; ch++){
                cout<<ch<< " ";
            }
            cout<< "\n";
        }
    }