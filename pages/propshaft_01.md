# Replacing Sprockets with Propshaft

* Railsがサポートするasset pipeline libraryがPropshaftのみに
  * 7.2まではオプションでSprockets、Propshaftを指定出来たが、8.0からSprocketsのサポートは削除され、選択出来なくなった
* Propshaftはリリースされた時から基本的には変わっておらず、assetsのload pathの対応と、assetsへのdigestの付与がメイン機能
* それ以外の機能、例えば、Javascriptのバンドル等は提供されない
  * 必要に応じて、jsbundling-railsやcssbundling-railsを使う必要がある
