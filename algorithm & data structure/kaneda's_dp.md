# kaneda's_algorithm

最大部分配列

``` ruby
def sub_max_array(nums)
  max_s = nums[0]
  s = nums[0]
  
  nums[1..nums.size].each do |num|
    s = [num, num+s].max
    max_s = s if s > max_s
  end
end

nums = [[-2,1,-3,4,-1,2,1,-5,4]
sub_max_array(nums)

#=> 6
```
