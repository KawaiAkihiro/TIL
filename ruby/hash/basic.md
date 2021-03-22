# hashの宣言

```ruby
  hash = {}
  hash[0] = "hello"
  #=> key = 0, value = "hello"
  
  hash[:a] = "world"
  #=> key = :a, value = "world"
  
  hash["test"] = 3
  #=> key = "test", value = 3
  
  p　hash
  #=> {0 => "hello", :a => "world", "test" => 3}
```

# hashのsort

例) valueの昇順にsort
```ruby
  hash = {0=>2, 1=>4, 2=>1, 3=>2, 4=>5}
  new_hash = hash.sort_by{|key, value| value}.to_h
  p new_hash
  #=> {2=>1, 0=>2, 3=>2, 1=>4, 4=>5}
```
ポイント：sort_byで一度key,valueが配列に変換されるのでto_hをしてもう一度ハッシュ化してやる必要がある

### to_h

```ruby
  p [0,1].to_h
  #=> {0=>1}
```

# .keys
ハッシュのキーだけを取り出して配列化するメソッド

```ruby
p new_hash.leys

#=> [2,0,3,1,5]
```

