## Pattern 11:


Sample Input 3 :

7

Sample Output 3 :


    A
    A B
    A B C 
    A B C D
    A B C D E
    A B C D E F
    A B C D E F G

## Solution in C++ :

    void nLetterTriangle(int n) {
        for(int i=0; i<n; i++){
            for(char ch='A'; ch <='A'+i;ch++){
                cout<< ch<< " ";
            }
            cout<< endl;
        }
    }