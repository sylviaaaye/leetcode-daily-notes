# 代码随想录算法day1|704. 二分查找 & 27. 移除元素 & 977.有序数组的平方

## 今日刷题列表
- [704. 二分查找](https://leetcode.cn/problems/binary-search/description/) - 难度1
- [27. 移除元素](https://leetcode.cn/problems/remove-element/) - 难度1
- [977.有序数组的平方 ](https://leetcode.cn/problems/squares-of-a-sorted-array/description/) - 难度0

## 每题总结

### 题目1
- 解题思路：
- 易错点/注意点：
- 代码实现：

```cpp
class Solution {
public:
    int search(vector<int>& nums, int target) {
        int mid = (nums.size()-1)/2;
        int begin = 0;
        int end = nums.size()-1;
        while(begin<=end){
            if(target == nums[mid]){
                return mid;}
            else if(target <nums[mid]){
                end = mid;
                mid = begin + (mid- begin) / 2;
            }
            else{
                begin = mid;
                mid = end - (end-mid)/2;
            }
    }
    return -1;}
};
```

- 复盘与提升：没做对，时间复杂度超时，答案边界也没搞好

---

### 题目2
- 解题思路：
- 易错点/注意点：
- 代码实现：

```cpp
class Solution {
public:
    int removeElement(vector<int>& nums, int val) {
        int slow, fast;
        slow = 0;
        int k = 0 ;
        for(int fast = 0; fast<nums.size(); fast++){
            if(nums[fast] == val){
                continue;
            }else{
                nums[slow++] == nums[fast];
                k++;
            }
        }
        return k;
    }
};
```

- 复盘与提升：答案出错，没看为啥

---

### 题目3
- 解题思路：
- 易错点/注意点：
- 代码实现：

```cpp
class Solution {
public:
    vector<int> sortedSquares(vector<int>& nums) {
        for(int i = 0; i<nums.size();i++){
            nums[i] = nums[i] * nums[i];
        }
        sort(nums.begin(), nums.end());
        return nums;
    }
};
```

- 复盘与提升：sort走天下，但是不会库函数

---

## 今日总结
- 学习时长：
- 收获：
- 困难：
1.什么算法是时间复杂度ologn的
