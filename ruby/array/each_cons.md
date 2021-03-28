# Array.each_cons(n)

n <= Array.size

Arrayからn個の要素を取り出して0からループする、終了はn個のペアが継続できるまで

```ruby
array = [1,2,3,4,5]
array.each_cons(3) do |x,y,z|
  p "#{x} #{y} #{z}
end

# 1 2 3
# 2 3 4
# 3 4 5
#この次は 4 5 ? となるので上記で繰り返しを終わる。
```
