## Reverse an Array

You are given an array of integers arr[]. Your task is to reverse the given array.

Examples:

    Input: arr = [1, 4, 3, 2, 6, 5]
    Output: [5, 6, 2, 3, 4, 1]

## solution in c++ :

    void reverseArray(vector<int> &arr) {
        // code here
        if(arr.empty()){
            cout<<"";
        }
        else{
            cout<<arr[arr.size()-1]<<" ";
            arr.pop_back();
            reverseArray(arr);
        }
    }
