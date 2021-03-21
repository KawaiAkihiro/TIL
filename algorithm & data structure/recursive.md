# 再起関数

関数aの中で関数aを使いどんどん階層を下げることで計算を楽にしてくれる

例題 与えられた数字nを1or2で表すときの組み合わせられる数(fibonacci数列)

```ruby
def answer(n)
  @cache = [1]
  memoize(n)
end

def memoize(n)
  return 0 if 0 > n 
  return @cache[n] if @cache[n]
  @cache[n] = memoize(n-2) + memoize(n-1)
end
```
