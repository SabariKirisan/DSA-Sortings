## Merge sort (c++)
Given an array arr[], its starting position l and its ending position r. Sort the array using the merge sort algorithm.

Input: arr[] = [4, 1, 3, 9, 7]
Output: [1, 3, 4, 7, 9]

## PROGRAM:(Main.cpp)
```
class Solution {
  public:
    void ms(vector<int>& arr,int l,int mid,int r)
    {
        vector<int> temp;
        int low=l;
        int high=mid+1;
        while(low<=mid && high<=r)
        {
            if(arr[low]<=arr[high])
            {
                temp.push_back(arr[low]);
                low++;
            }
            else 
            {
                temp.push_back(arr[high]);
                high++;
            }
        }
        while(low<=mid)
        {
            temp.push_back(arr[low]);
            low++;
        }
        while(high<=r)
        {
            temp.push_back(arr[high]);
            high++;
        }
        for (int i = 0; i < temp.size(); i++)
        {
        arr[l + i] = temp[i]; 
        }
    }
  
  
    void mergeSort(vector<int>& arr, int l, int r) 
    {
         if(l>=r) return;
         int mid=(l+r)/2;
         mergeSort(arr,l,mid);
         mergeSort(arr,mid+1,r);
         ms(arr,l,mid,r);
    }
};
```
## Complexity
- Time complexity : O(nlogn)

- Space complexity : O(n)

## OUTPUT
Output: [1, 3, 4, 7, 9]
