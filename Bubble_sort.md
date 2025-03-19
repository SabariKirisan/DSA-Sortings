## Bubble sort (c++)
Given an array, arr[]. Sort the array using bubble sort algorithm.

Input: arr[] = [4, 1, 3, 9, 7]

Output: [1, 3, 4, 7, 9]

## PROGRAM:(Main.cpp)
```
class Solution {
  public:
    // Function to sort the array using bubble sort algorithm.
    void bubbleSort(vector<int>& arr) {
        int n=arr.size();
        for (int i=0;i<n-1;i++)
        {
            int swap=0;
            for (int j=0;j<n-i-1;j++)
            {
                if(arr[j+1]<arr[j])
                {
                    int temp=arr[j+1];
                    arr[j+1]=arr[j];
                    arr[j]=temp;
                    swap=1;
                   
                }
            }
            if(swap==0)
            {
                break;
            }
        }
    }
};
```
## Complexity
- Time complexity : Worst-case and Average-case O(n 2 ) best case O(n)

- Space complexity : O(1)

## OUTPUT
Output: [1, 3, 4, 7, 9]
