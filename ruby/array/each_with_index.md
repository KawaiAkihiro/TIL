# each_with_index(num, i)
配列の中身とインデックスを両方使った繰り返し文
numが中身,iがインデックス

```ruby
samples = [1,2,3,4,5]
samples.each_with_index |sample, i|
  puts "#{i}番目は#{sample}"
end
#=> 
#0番目は1
#1番目は2
#2番目は3
#3番目は4
#4番目は5
```
