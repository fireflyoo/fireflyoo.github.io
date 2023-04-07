---
title: "[LeetCode]78.子集,90.子集II"
date: 2023-04-07
author: fireflyoo
---
子集
===
## 问题描述
这道题是 LeetCode 78 题 - 子集。

从不含重复元素的 n 个元素中，选择 0~n 个元素，组成一个子集，找出所有的子集（幂集）。
## 解法一：二进制转换法
```ruby
def subsets(nums)
    Array.new(1<<nums.size){|mask|
        nums.filter.with_index{|n,i|
            mask&(1<<i)>0
        }
    }
end
```
时间复杂度：O(n×2^n)  
空间复杂度：O(n)  
## 解法二：递归
```ruby
def subsets(nums)
    return [[]] if nums==[]
    sub=subsets(nums[1..])
    sub+sub.map{|n|[nums[0],*n]}
end
```
时间复杂度：  
空间复杂度：  
## 解法三：回溯-二叉树
```ruby
def subsets(nums,path=[])
    return [path] if nums==[]
    subsets(nums[1..],[nums[0],*path])+subsets(nums[1..],path)
end
```
## 解法四：逐个枚举法
```ruby
def subsets(nums)
    nums.reduce([[]]){|res,n|
        res.reduce(res){|ans,m|
            ans+[[n,*m]]
        }
    }
end
```

