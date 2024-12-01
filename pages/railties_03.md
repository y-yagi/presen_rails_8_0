# Add script folder and generator

* [PR](https://github.com/rails/rails/pull/52335)
* `script`を生成する為のgeneratorを追加
* `script`はデータマイグレーションやデータのクリーンアップなど、一度だけ実行したい、または汎用的に使用する、Rubyのスクリプトを格納する為に使用する事を想定している、との事
* generatorが生成するコードは下記

```ruby
require_relative "../config/environment"

# Your code goes here
```
Add internal page `/rails/info/notes`
