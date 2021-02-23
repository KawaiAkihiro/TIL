#子モデルのdependent設定

## :destroy、:delete_all

```ruby
class Parent < ApplicationRecord
   has_many :childs, dependent: :destroy(or :delete_all)
end
```

Parentモデルが削除されたらChildモデルのデータも消える
違いはログが出るか出ないか、クエリの回数

## :nillity

```ruby
class Parent < ApplicationRecord
   has_many :childs, dependent: :nillity
end
```

Parentモデルが削除されたらChildモデルはparent_idがnilになる
