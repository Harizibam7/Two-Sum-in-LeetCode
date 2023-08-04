# Two-Sum-in-LeetCode


Two Sum in LeetCode By using C 


    #include<stdio.h>
    int* twoSum(int* nums, int numsSize, int target, int* returnSize){
        int *arr= malloc(2*sizeof(int));
        *returnSize =2;
        for(int i = 0;i<numsSize;i++){
            for(int j=i+1;j<numsSize;j++){
                if(nums[i]+nums[j]==target){
                    arr[0] = i;
                    arr[1] = j;
    
                }
            }
        }
    
        return arr;
    }

Two Sum in LeetCode By using C++

    class Solution {
    public:
        vector<int> twoSum(vector<int>& nums, int target) {
            for( int i= 0;i<nums.size(); i++){
                for(int j=i+1;j<nums.size();j++){
                    if(nums[i]+nums[j]==target){
                        return{i,j};
                    }
                }
            }
            return{};
        }
    };
