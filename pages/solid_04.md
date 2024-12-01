# Solid Cache

* [Active Support Cache Store](https://api.rubyonrails.org/classes/ActiveSupport/Cache/Store.html)のキャッシュストアにRDBMSを使用出来るようにしたライブラリ
  * Railsが標準でサポートしているストレージは、メモリ、ファイル、memcached、Redisだけだった
  * RDBMSをサポートしている[3rd partyのライブラリ](https://github.com/bsm/activesupport-cache-database)はあった
