# A Solid Reduction of Dependencies

* 従来のRailsでは、一部コンポーネントを使用するのに特定のサービスに依存していた
  * 例えば、Action Cableを使用するには、RedisかPostgreSQLが必要だった
* Rails 8.0では、新しくSolid Cable、Solid Cable、Solid Queueという3つのgem(通称Solid Trifecta)が追加されて、特定のサービスに依存せずにRailsの全ての機能が使えるようになった
  * Redis無しでSQLite3だけでも大丈夫
