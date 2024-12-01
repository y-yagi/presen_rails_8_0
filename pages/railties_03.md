# [Add script folder and generator (#52335)](https://github.com/rails/rails/commit/c01a8466581b69d7886fb926ede5e76a74395162)

* `script`を生成する為のgeneratorを追加
* `script`はデータマイグレーションやデータのクリーンアップなど、一度だけ実行したい、または汎用的に使用する、Rubyのスクリプトを格納する為に使用する事を想定している、との事
* generatorが生成するコードは下記

```ruby
require_relative "../config/environment"

# Your code goes here
```
