# Kamal

* コンテナ用のCapistrano
* ゼロダウンタイムのデプロイ、ローリングリスタート、アセットブリッジング、リモートビルドなどを提供
  * Kamal経由でサーバへのbashやRails consoleの実行なども出来る
* 必要なのはSSH接続出来るユーザと、Docker Registryへの情報のみ
  * コンテナイメージのpush/pullを行う為、Registryの情報が必要
* `kamal setup`でセットアップをしたら、後は`kamal deploy`すればデプロイ出来る