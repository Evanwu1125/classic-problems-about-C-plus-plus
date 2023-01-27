输入一个数组和一个数字 s
，在数组中查找两个数，使得它们的和正好是 s
。

如果有多对数字的和等于 s
，输出任意一对即可。

你可以认为每组输入中都至少含有一组满足条件的输出。

### 数据范围
数组长度 [1,1002]
。

### 样例
输入：[1,2,3,4] , sum=7

输出：[3,4]
```c++
class Solution {
public:
    vector<int> findNumbersWithSum(vector<int>& nums, int target) {
        unordered_set<int> S;
        for (auto x : nums)
        {
            if (S.count(target - x)) return {x, target - x};
            S.insert(x);
        }        
    }
};
```
