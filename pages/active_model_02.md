# Add `:except_on` option for validations

* [PR](https://github.com/rails/rails/pull/43495)
* 特定のcontextの場合のみバリデーションをスキップ出来るようにする為の`:except_on`オプションを追加

```ruby
class User < ApplicationRecord
  validates :birthday, presence: { except_on: :admin }
end

user = User.new
user.save(context: :admin) # `birthday`に関するバリデーションが実行されない
```
