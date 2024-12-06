# Add not-null type modifier to migration attributes

* [PR](https://github.com/rails/rails/pull/52327)
* カラムのnot-null制約をgeneratorで指定出来るよう対応
* not-nullにしたい場合、型の末尾に`!`をつければ良い

```bash
bin/rails generate migration CreateUsers email_address:string!:uniq password_digest:string!
```

```ruby
class CreateUsers < ActiveRecord::Migration[8.0]
  def change
    create_table :users do |t|
      t.string :email_address, null: false
      t.string :password_digest, null: false

      t.timestamps
    end
    add_index :users, :email_address, unique: true
  end
end
```
