# bsearch

(0...10)bsearch{ |i| #ここに入る条件を満たす最初のiを返す}

example

```ruby
  array = [0,1,4,7,10]
  (0...array.size).bsearch{|x| array[x] >= 3} #=> 2(条件を満たす最初のindex)
  (0...array.size).bsearch{|x| array[x] - 7}  #=> 3(式のみの記述の場合"式 == 0"となるindexを探す)  
```

# おまけ知識

```{ }```の中身が不等号のないただの式の場合**式 == 0**となるものを範囲(or配列)の中から探す
