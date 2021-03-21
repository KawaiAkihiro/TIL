# slice(range)
文字列の特定範囲のみの文字だけ返すメソッド

```ruby
str = "hello!!"
puts str.slice(0..3)
=> "hell"
```

# 文字列でもincludeは使える
配列でよく見かけるincludeは文字列を対象にしても問題ない。

```ruby
str = "hello"
str.include?("o")

=> true
```
