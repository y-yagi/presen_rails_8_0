# Support batching using custom columns

* [PR](https://github.com/rails/rails/pull/52384)
* バッチ系のメソッド(例：`in_batches`)でデータ取得時の条件に使用するカラムがプライマリーキー固定だったのを、任意のカラムを指定できるよう対応

```ruby
Product.in_batches(cursor: [:shop_id, :id]) do |relation|
  # ...
end
```

* カラムは複数指定できるが、プライマリーキーなどのユニークなカラムが必ず指定されている必要がある