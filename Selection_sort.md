## Selection sort (c++)
Given an array arr, use selection sort to sort arr[] in increasing order.

Input: arr[] = [4, 1, 3, 9, 7]
Output: [1, 3, 4, 7, 9]

## PROGRAM:(Main.cpp)
```
class Solution {
  public:
    // Function to perform selection sort on the given array.
    void selectionSort(vector<int> &arr) {
        
        int n=arr.size();
        for(int i=0;i<n-1;i++){
            for(int j=i+1;j<n;j++)
            {
                if(arr[i]>arr[j]){
                    swap(arr[i],arr[j]);
                }
            }
            
        }
    }
};
```
- Time complexity : O(n2)

- Space complexity : O(1)

## OUTPUT
Output: [1, 3, 4, 7, 9]

