# 文字列の連結

## "+"

```ruby
puts "abc" + "def"
=> "abcdef"
```

## << 

```ruby
puts "abc" << "def"
=> "abcdef"
```

## (Str).concat()

```ruby
puts "abc".concat("def")
=> "abcdef"
```

# 文字列の削除

## (Str).chop

```ruby
puts "abc".chop
=> "ab"
#最後の１文字を削除する
```

## (Str).delete()

```ruby
puts "abcdef".delete("def")
=> "abc"
#指定した文字列を削除する
```
