# Contains Duplicate
Easy - Given an integer array nums, return true if any value appears more than once in the array, otherwise return false.

https://neetcode.io/problems/duplicate-integer

# Solution
```
class Solution {
public:
    bool hasDuplicate(vector<int>& nums) {
        unordered_set<int> set;
        for(int num : nums){
            if(set.find(num) != set.end())
                return true;
            set.insert(num);
        }
        return false;
    }
};
```

## Video solution
https://www.youtube.com/watch?v=3OamzN90kPg

