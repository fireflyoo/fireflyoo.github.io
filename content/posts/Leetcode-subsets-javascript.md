---
title: "[LeetCode][Javascript]78.子集,90.子集II"
date: 2024-04-23
author: fireflyoo
---
子集
===
## 问题描述
这道题是 LeetCode 78 题 - 子集。

从不含重复元素的 n 个元素中，选择 0~n 个元素，组成一个子集，找出所有的子集（幂集）。

## 解法一：回溯-多叉树
```javascript
/**
 * @param {number[]} nums
 * @return {number[][]}
 */
const dfs = function* (nums,i=0,path=[]) {
    yield path
    for(let j=i;j<nums.length;j++){
        yield* dfs(nums,j+1,path.concat(nums[j]))
    }
};
const subsets=nums=>[...dfs(nums)]
```
时间复杂度：  
空间复杂度：  
## 解法二：回溯-二叉树
```javascript
/**
 * @param {number[]} nums
 * @return {number[][]}
 */
const dfs = function* (nums,i=0,path=[]) {
    if(nums.length==i){
        yield path
    } else {
        yield* dfs(nums,i+1,path)
        yield* dfs(nums,i+1,path.concat(nums[i]))
    }
};
const subsets=nums=>[...dfs(nums)]
```

## 解法三：逐个枚举法
## 解法四：
