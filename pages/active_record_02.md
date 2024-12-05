# Allow `ActiveRecord::Base#pluck` to accept hash arguments with symbol and string values.

* [PR](https://github.com/rails/rails/pull/51676)
* 特定のテーブルのカラムを1つだけ`pluck`で取得したい場合に、arrayを指定する必要があったのを、string、symbolで取得できるよう対応

```ruby
# before
Post.joins(:comments).pluck(:id, comments: [:id])

# after
Post.joins(:comments).pluck(:id, comments: :id)
Post.joins(:comments).pluck("id", "comments" => "id")
```