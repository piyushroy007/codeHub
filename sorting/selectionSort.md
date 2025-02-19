## Selection Sort

The algorithm steps are as follows:

    1) First, we will select the range of the unsorted array using a loop (say i) that indicates the starting index of the range.
    2) The loop will run forward from 0 to n-1. The value i = 0 means the range is from 0 to n-1, and similarly, i = 1 means the range is from 1 to n-1, and so on.
    (Initially, the range will be the whole array starting from the first index.)
    3)Now, in each iteration, we will select the minimum element from the range of the unsorted array using an inner loop.
    4)After that, we will swap the minimum element with the first element of the selected range(in step 1).
    Finally, after each iteration, we will find that the array is sorted up to the first index of the range.

## Input:

    arr[] = [4, 1, 3, 9, 7]

## Output:

    [1, 3, 4, 7, 9]

## solution in c++ :

    void selectionSort(vector<int> &arr) {
        // code here
        for(int i=0;i<arr.size()-1;i++){
            int min=arr[i];
            for(int j=i+1;j<arr.size();j++){
                if(arr[j]<min){
                    min=arr[j];
                    arr[j]=arr[i];
                    arr[i]=min;
                }
            }
        }
    }
