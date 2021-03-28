# select

配列の中から条件を満たす要素だけを返すメソッド

```ruby
  array = [1,2,3,4,5,6]
  puts array.select{|x| x % 2 == 0}
  #=> [2,4,6]
```
