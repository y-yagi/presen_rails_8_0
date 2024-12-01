# [Add `:except_on` option for validations](https://github.com/rails/rails/commit/372c64294b3baaf9a691d233c75d6a97a373f483)

* 特定のcontextの場合のみバリデーションをスキップ出来るようにする為の`:except_on`オプションを追加

```ruby
class User < ApplicationRecord
  validates :birthday, presence: { except_on: :admin }
end

user = User.new
user.save(context: :admin) # `birthday`に関するバリデーションが実行されない
```
