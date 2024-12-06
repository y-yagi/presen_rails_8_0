# A Solid Reduction of Dependencies

* 従来のRailsでは、一部コンポーネントを使用するのに特定のサービスに依存していた
  * 例えば、Action Cableを使用するには、RedisかPostgreSQLが必要だった
* Rails 8.0では、新しくSolid Cable、Solid Cable、Solid Queueという3つのgem(通称Solid Trifecta)が追加されて、RailsがサポートしているRDBMSだけあれば、Railsの全ての機能が使えるようになった
  * SQLiteだけでも大丈夫
* Rails 8.0で新規にアプリケーションを作成した場合、Solid Trifectaを使うよう設定されるようになっている