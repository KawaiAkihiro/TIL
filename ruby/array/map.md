# map

配列の各要素に対して行うメソッド
mapは結果を保持する。eachは計算するだけ

```ruby
def map_sample(a)
   a.map{|num| num*2}
end

nums = [1,2,3,4]
puts map_sample(nums)

#=> [2,4,6,8]
```
