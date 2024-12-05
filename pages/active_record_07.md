# Allow `drop_table` to accept an array of table names

* [PR](https://github.com/rails/rails/pull/52773)
* `drop_table`にテーブル名を複数指定できるようになった

```ruby
drop_table(:users, :posts)
```