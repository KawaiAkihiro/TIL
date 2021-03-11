# 構造体(struct)

特定のデータの集まり

## 定義の仕方

```ruby
User = Struct.new(:name, :age)
puts User.new("kawai", 23) #=> struct User name="kawai" age=23
```

```ruby
user1 = User.new("akihiro",23)
#参照
puts user1.name #=> "akihiro"
#更新
user1.age = 24
puts user1.age #=> 24
```

# Float::INFINITY
不動小数点における正の最大値

# to_a 
配列化するメソッド

```ruby
puts (1..3).to_a #=> [1,2,3]
```

# range
数値の範囲を決める

```ruby
(1..4).each |index|
  puts "数値は#{index}"
end
#=> 
#数値は１
#数値は２
#数値は３
#数値は４
```

# reverse_each
降順のループ文

```ruby
(1..4)reverse_each |index|
  puts "数値は#{index}"
end
#=> 
#数値は4
#数値は3
#数値は2
#数値は1
```

