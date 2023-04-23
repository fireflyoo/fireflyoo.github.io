---
title: "[LeetCode][Elixir]78.子集,90.子集II"
date: 2023-04-23
author: fireflyoo
---
子集
===
## 问题描述
这道题是 LeetCode 78 题 - 子集。

从不含重复元素的 n 个元素中，选择 0~n 个元素，组成一个子集，找出所有的子集（幂集）。
## 解法一：二进制转换法
```elixir
import Bitwise
defmodule Solution do
  @spec subsets(nums :: [integer]) :: [[integer]]
  def subsets(nums) do
    n=length nums
    for mask <- (0..(1 <<< n)-1) do
        for {num,i} <- Enum.with_index(nums) ,(mask &&& (1 <<< i)) > 0   do
            num
        end
    end
  end
end
```
时间复杂度：O(n×2^n)  
空间复杂度：O(n)  
## 解法二：递归
```elixir
defmodule Solution do
  @spec subsets(nums :: [integer]) :: [[integer]]
  def subsets([]), do: [[]]
  def subsets([num|tail]) do
    sub=subsets(tail)
    sub++Enum.map sub,&[num|&1]
  end
end
```
时间复杂度：  
空间复杂度：  
## 解法三：回溯-二叉树
```elixir
defmodule Solution do
  @spec subsets(nums :: [integer]) :: [[integer]]
  def subsets([],path), do: [path]
  def subsets([num|tail],path \\ []) do
    subsets(tail,path)++subsets(tail,[num|path])
  end
end
```

## 解法四：逐个枚举法
```elixir
defmodule Solution do
  @spec subsets(nums :: [integer]) :: [[integer]]
  def subsets(nums) do
    for num <- nums, reduce: [[]] do
        res -> 
            for m <- res, reduce: res do
                ans ->
                    [[num|m]|ans]
            end
    end
  end
end
```
## 解法五：逐个枚举法-尾递归版
```elixir
# 尾递归版本
defmodule Solution do
  @spec subsets(nums :: [integer]) :: [[integer]]
  def subsets([],q,sum), do: sum
  def subsets([num|tail],[],sum), do: subsets(tail,sum,sum)
  def subsets(nums,[q0|q_tail] \\ [[]],sum \\ [[]]) do
    subsets(nums,q_tail,[[hd(nums)|q0]|sum])
  end
end
```
