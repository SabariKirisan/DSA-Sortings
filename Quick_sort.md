## Quick sort (c++)
Implement Quick Sort, a Divide and Conquer algorithm, to sort an array, arr[] in ascending order. Given an array, arr[], with starting index low and ending index high, complete the functions partition() and quickSort(). Use the last element as the pivot so that all elements less than or equal to the pivot come before it, and elements greater than the pivot follow it.

Note: The low and high are inclusive.
Input: arr[] = [4, 1, 3, 9, 7]
Output: [1, 3, 4, 7, 9]

## PROGRAM:(Main.cpp)
```
class Solution {
  public:
    // Function to sort an array using quick sort algorithm.
    void quickSort(vector<int>& arr, int low, int high) {
        if(low<high)
        {
            int pindex=partition(arr,low,high);
            quickSort(arr,low,pindex-1);
            quickSort(arr,pindex+1,high);
            
        }
    }

  public:
    int partition(vector<int>& arr, int low, int high) {
        int pivot=arr[low];
        int i=low;
        int j=high;
        while(i<j)
        {
            while(arr[i]<=pivot && i<high)
            {
                i++;
            }
            while(arr[j]>pivot && j>low)
            {
                j--;
            }
            if(i<j) swap(arr[i],arr[j]);
        }
        swap(arr[low],arr[j]);
        return j;
    }
};
```

## Complexity
- Time complexity :Best-case and Average-case Time Complexity: O(nlogn)

Worst-case Time Complexity: O(n2) (when the pivot is poorly chosen)

- Space complexity : Best/Average case: O(logn) (due to recursion depth)

Worst case: O(n) (unbalanced recursion)

## OUTPUT
Output: [1, 3, 4, 7, 9]
